<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section
      class="section-padding bg-gradient-to-br from-primary-50 via-white to-purple-50 dark:from-dark-900 dark:via-dark-800 dark:to-dark-900">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto text-center">
          <h1 class="text-5xl md:text-6xl font-bold mb-6 animate-slide-up">
            {{ $t('contact.title') }}
          </h1>
          <p class="text-xl text-gray-600 dark:text-gray-400 mb-8 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('contact.subtitle') }}
          </p>
        </div>
      </div>
    </section>

    <!-- Contact Information -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="max-w-6xl mx-auto">
          <div class="grid lg:grid-cols-2 gap-12">
            <!-- Contact Info -->
            <div class="animate-slide-left">
              <h2 class="text-3xl font-bold mb-8">{{ $t('contact.letsConnect') }}</h2>
              <p class="text-lg text-gray-600 dark:text-gray-400 mb-8 leading-relaxed">
                {{ $t('contact.description') }}
              </p>

              <div class="space-y-6">
                <div class="flex items-center">
                  <div
                    class="w-12 h-12 bg-primary-100 dark:bg-primary-900 rounded-lg flex items-center justify-center mr-4">
                    <PhoneIcon class="w-6 h-6 text-primary-600 dark:text-white" />
                  </div>
                  <div>
                    <p class="font-medium text-gray-900 dark:text-white">{{ $t('contact.phone') }}</p>
                    <p class="text-gray-600 dark:text-gray-400">+216 25834026</p>
                  </div>
                </div>

                <div class="flex items-center">
                  <div
                    class="w-12 h-12 bg-primary-100 dark:bg-primary-900 rounded-lg flex items-center justify-center mr-4">
                    <EnvelopeIcon class="w-6 h-6 text-primary-600 dark:text-white" />
                  </div>
                  <div>
                    <p class="font-medium text-gray-900 dark:text-white">{{ $t('contact.email') }}</p>
                    <p class="text-gray-600 dark:text-gray-400">sayahayoub9827@gmail.com</p>
                  </div>
                </div>

                <div class="flex items-center">
                  <div
                    class="w-12 h-12 bg-primary-100 dark:bg-primary-900 rounded-lg flex items-center justify-center mr-4">
                    <MapPinIcon class="w-6 h-6 text-primary-600 dark:text-white" />
                  </div>
                  <div>
                    <p class="font-medium text-gray-900 dark:text-white">{{ $t('contact.location') }}</p>
                    <p class="text-gray-600 dark:text-gray-400">Sousse, Tunisia</p>
                  </div>
                </div>
              </div>

              <div class="mt-8">
                <h3 class="text-xl font-bold mb-4">{{ $t('contact.followMe') }}</h3>
                <div class="flex space-x-4">
                  <a href="https://github.com/ayoubsayah" target="_blank" rel="noopener noreferrer"
                    class="w-12 h-12 bg-gray-100 dark:bg-gray-800 rounded-lg flex items-center justify-center hover:bg-primary-100 dark:hover:bg-primary-900 transition-colors duration-200">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                      <path
                        d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
                    </svg>
                  </a>
                  <a href="https://linkedin.com/in/ayoubsayah" target="_blank" rel="noopener noreferrer"
                    class="w-12 h-12 bg-gray-100 dark:bg-gray-800 rounded-lg flex items-center justify-center hover:bg-primary-100 dark:hover:bg-primary-900 transition-colors duration-200">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                      <path
                        d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z" />
                    </svg>
                  </a>
                </div>
              </div>
            </div>

            <!-- Contact Form -->
            <div class="animate-slide-right">
              <div class="card p-8">
                <h3 class="text-2xl font-bold mb-6">{{ $t('contact.sendMessage') }}</h3>

                <form @submit.prevent="handleSubmit" class="space-y-6">
                  <div class="grid md:grid-cols-2 gap-6">
                    <div>
                      <label for="firstName" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                        {{ $t('contact.firstName') }}
                      </label>
                      <input type="text" id="firstName" v-model="form.firstName"
                        class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent dark:bg-gray-800 dark:text-white"
                        required>
                    </div>
                    <div>
                      <label for="lastName" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                        {{ $t('contact.lastName') }}
                      </label>
                      <input type="text" id="lastName" v-model="form.lastName"
                        class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent dark:bg-gray-800 dark:text-white"
                        required>
                    </div>
                  </div>

                  <div>
                    <label for="email" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                      {{ $t('contact.email') }}
                    </label>
                    <input type="email" id="email" v-model="form.email"
                      class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent dark:bg-gray-800 dark:text-white"
                      required>
                  </div>

                  <div>
                    <label for="subject" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                      {{ $t('contact.subject') }}
                    </label>
                    <input type="text" id="subject" v-model="form.subject"
                      class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent dark:bg-gray-800 dark:text-white"
                      required>
                  </div>

                  <div>
                    <label for="message" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-2">
                      {{ $t('contact.message') }}
                    </label>
                    <textarea id="message" v-model="form.message" rows="5"
                      class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent dark:bg-gray-800 dark:text-white"
                      required></textarea>
                  </div>

                  <button type="submit" :disabled="isSubmitting"
                    class="w-full btn-primary py-3 text-lg font-semibold disabled:opacity-50 disabled:cursor-not-allowed">
                    <span v-if="isSubmitting">{{ $t('contact.sending') }}</span>
                    <span v-else>{{ $t('contact.send') }}</span>
                  </button>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Availability Section -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto text-center">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('contact.currentAvailability') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 mb-8 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('contact.availabilityDesc') }}
          </p>

          <div class="grid md:grid-cols-3 gap-8">
            <div class="card p-6 text-center animate-slide-up">
              <div class="text-3xl font-bold gradient-text mb-2">{{ $t('contact.availableForProjects') }}</div>
              <p class="text-gray-600 dark:text-gray-400">{{ $t('contact.projects') }}</p>
            </div>

            <div class="card p-6 text-center animate-slide-up" style="animation-delay: 0.1s;">
              <div class="text-3xl font-bold gradient-text mb-2">{{ $t('contact.fullTime') }}</div>
              <p class="text-gray-600 dark:text-gray-400">{{ $t('contact.employment') }}</p>
            </div>

            <div class="card p-6 text-center animate-slide-up" style="animation-delay: 0.2s;">
              <div class="text-3xl font-bold gradient-text mb-2">{{ $t('contact.contract') }}</div>
              <p class="text-gray-600 dark:text-gray-400">{{ $t('contact.opportunities') }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import { PhoneIcon, EnvelopeIcon, MapPinIcon } from '@heroicons/vue/24/outline'

const form = ref({
  firstName: '',
  lastName: '',
  email: '',
  subject: '',
  message: ''
})

const isSubmitting = ref(false)

const handleSubmit = async () => {
  isSubmitting.value = true
  fetch('https://formspree.io/f/xeolkdvl', {
    method: 'POST',
    headers: {
      'Accept': 'application/json',
      'Content-Type': 'application/json'
    },
    body: JSON.stringify({
      ...form.value
    })
  })
    .then(response => response.json())
    .then(data => {
      isSubmitting.value = false
      alert('Message sent successfully!')

    })
    .catch(error => {
      console.error('Error:', error)
    })
  // Simulate form submission

  // Reset form
  form.value = {
    firstName: '',
    lastName: '',
    email: '',
    subject: '',
    message: ''
  }


  // Show success message (you can implement a toast notification here)
}
</script>
