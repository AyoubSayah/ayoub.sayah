<script setup lang="ts">
import { ref, onMounted, computed } from 'vue'
import { useI18n } from 'vue-i18n'
import { SunIcon, MoonIcon, Bars3Icon } from '@heroicons/vue/24/outline'

const { locale } = useI18n()

const isDark = ref(false)
const mobileMenuOpen = ref(false)

const currentLanguage = computed(() => locale.value)

const navItems = [
  { path: '/', key: 'home' },
  { path: '/about', key: 'about' },
  { path: '/experience', key: 'experience' },
  { path: '/projects', key: 'projects' },
  { path: '/skills', key: 'skills' },
  { path: '/contact', key: 'contact' }
]

const toggleTheme = () => {
  isDark.value = !isDark.value
  localStorage.setItem('theme', isDark.value ? 'dark' : 'light')
  applyTheme()
}

const applyTheme = () => {
  if (isDark.value) {
    document.documentElement.classList.add('dark')
  } else {
    document.documentElement.classList.remove('dark')
  }
}

const toggleLanguage = () => {
  locale.value = locale.value === 'en' ? 'fr' : 'en'
  localStorage.setItem('locale', locale.value)
}

const toggleMobileMenu = () => {
  mobileMenuOpen.value = !mobileMenuOpen.value
}
// function handleKey(e) {
//   switch (e.key) {
//     case "ArrowLeft":
//       alert("left");
//       break;
//     case "ArrowRight":
//       alert("right");
//       break;
//     case "+":
//       alert("plus");
//       break;
//     case "-":
//     case "Delete":

//       break;
//   }
// }

// onMounted(() => {
//   window.addEventListener("keyup", handleKey);
// });
// onBeforeUnmount(() => {
//   window.removeEventListener("keyup", handleKey);
// });
onMounted(() => {
  const savedTheme = localStorage.getItem('theme')
  if (savedTheme) {
    isDark.value = savedTheme === 'dark'
  } else {
    isDark.value = window.matchMedia('(prefers-color-scheme: dark)').matches
  }
  applyTheme()

  const savedLocale = localStorage.getItem('locale')
  if (savedLocale) {
    locale.value = savedLocale
  }
})
</script>

<template>
  <div id="app" class="min-h-screen bg-gray-50 dark:bg-dark-900 text-gray-900 dark:text-gray-100">
    <nav
      class="fixed top-0 w-full bg-white/80 dark:bg-dark-800/80 backdrop-blur-md z-50 border-b border-gray-200 dark:border-dark-700">
      <div class="container-custom">
        <div class="flex items-center justify-between h-16">
          <router-link to="/" class="text-2xl font-bold gradient-text">
            Ayoub Sayah
          </router-link>

          <div class="hidden md:flex items-center space-x-8">
            <router-link v-for="item in navItems" :key="item.path" :to="item.path" active-class="font-bold  underline"
              class="text-gray-600 dark:text-gray-300 hover:text-primary-600 dark:hover:text-primary-400 transition-colors duration-200"
              active>
              {{ $t(`nav.${item.key}`) }}
            </router-link>

            <!-- Language Switcher -->
            <button @click="toggleLanguage"
              class="flex cursor-pointer items-center space-x-2 text-gray-600 dark:text-gray-300 hover:text-primary-600 dark:hover:text-primary-400 transition-colors duration-200 border p-1 rounded">
              <span class="text-sm font-medium">{{ currentLanguage.toUpperCase() }}</span>
            </button>

            <!-- Theme Toggle -->
            <button @click="toggleTheme"
              class="p-2 rounded-lg cursor-pointer bg-gray-100 dark:bg-dark-700 hover:bg-gray-200 dark:hover:bg-dark-600 transition-colors duration-200">
              <SunIcon v-if="isDark" class="w-5 h-5 text-yellow-500" />
              <MoonIcon v-else class="w-5 h-5 text-gray-600" />
            </button>
          </div>

          <!-- Mobile menu button -->
          <button @click="toggleMobileMenu"
            class="md:hidden p-2 rounded-lg bg-gray-100 dark:bg-dark-700 hover:bg-gray-200 dark:hover:bg-dark-600 transition-colors duration-200">
            <Bars3Icon class="w-5 h-5" />
          </button>
        </div>

        <!-- Mobile menu -->
        <div v-if="mobileMenuOpen" class="md:hidden py-4 border-t border-gray-200 dark:border-dark-700">
          <div class="flex flex-col space-y-4">
            <router-link v-for="item in navItems" :key="item.path" :to="item.path" @click="mobileMenuOpen = false"
              class="text-gray-600 dark:text-gray-300 hover:text-primary-600 dark:hover:text-primary-400 transition-colors duration-200">
              {{ $t(`nav.${item.key}`) }}
            </router-link>

            <!-- Mobile Language Switcher -->
            <button @click="toggleLanguage"
              class="flex items-center space-x-2 text-gray-600 dark:text-gray-300 hover:text-primary-600 dark:hover:text-primary-400 transition-colors duration-200 border-2 border-white">
              <span class="text-lg">{{ currentLanguage === 'en' ? '🇺🇸' : '🇫🇷' }}</span>
              <span class="text-sm font-medium">{{ currentLanguage.toUpperCase() }}</span>
            </button>

            <!-- Mobile Theme Toggle -->
            <button @click="toggleTheme"
              class="flex items-center space-x-2 text-gray-600 dark:text-gray-300 hover:text-primary-600 dark:hover:text-primary-400 transition-colors duration-200">
              <SunIcon v-if="isDark" class="w-5 h-5 text-yellow-500" />
              <MoonIcon v-else class="w-5 h-5 text-gray-600" />
              <span>{{ isDark ? 'Light Mode' : 'Dark Mode' }}</span>
            </button>
          </div>
        </div>
      </div>
    </nav>

    <!-- Main content -->
    <main class="pt-16">
      <router-view v-slot="{ Component }">
        <transition name="page" mode="out-in">
          <component :is="Component" />
        </transition>
      </router-view>
    </main>

    <!-- Footer -->
    <footer class="bg-white dark:bg-dark-800 border-t border-gray-200 dark:border-dark-700 py-8">
      <div class="container-custom">
        <div class="text-center">
          <p class="text-gray-600 dark:text-gray-400">{{ $t('footer.copyright') }}</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<style>
/* Prevent flash of unstyled content */
html {
  transition: background-color 0.3s ease, color 0.3s ease;
}

/* Dark mode styles */
.dark {
  color-scheme: dark;
}

/* Page transitions */
.page-enter-active,
.page-leave-active {
  transition: all 0.3s ease;
}

.page-enter-from {
  opacity: 0;
  transform: translateX(20px);
}

.page-leave-to {
  opacity: 0;
  transform: translateX(-20px);
}
</style>
