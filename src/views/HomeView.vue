<script setup lang="ts">
import {
  CodeBracketIcon,
  GlobeAltIcon,
  CommandLineIcon,
  ServerIcon,
  CogIcon
} from '@heroicons/vue/24/outline'
</script>

<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section
      class="relative min-h-screen flex items-center justify-center overflow-hidden bg-gradient-to-br from-primary-50 via-white to-purple-50 dark:from-dark-900 dark:via-dark-800 dark:to-dark-900">
      <!-- Animated Background Elements -->
      <div class="absolute inset-0 overflow-hidden">
        <div
          class="absolute top-20 left-20 w-72 h-72 bg-primary-300 dark:bg-primary-700 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-float">
        </div>
        <div
          class="absolute top-40 right-20 w-96 h-96 bg-purple-300 dark:bg-purple-700 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-float"
          style="animation-delay: 2s;"></div>
        <div
          class="absolute bottom-20 left-1/2 w-80 h-80 bg-pink-300 dark:bg-pink-700 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-float"
          style="animation-delay: 4s;"></div>
      </div>

      <div class="container-custom relative z-10">
        <div class="max-w-4xl mx-auto text-center">
          <div class="animate-bounce-in">
            <p class="text-xl md:text-2xl text-primary-600 dark:text-primary-400 mb-4 animate-slide-down">
              {{ $t('home.greeting') }}
            </p>
            <h1 class="text-5xl md:text-7xl lg:text-8xl font-bold mb-6 animate-slide-up">
              <span class="gradient-text">Ayoub Sayah</span>
            </h1>
            <h2
              class="text-2xl md:text-3xl lg:text-2xl font-semibold mb-8 text-gray-700 dark:text-gray-300 animate-slide-up"
              style="animation-delay: 0.2s;">
              <span class="">{{ $t('home.title') }}</span>
            </h2>
            <p class="text-lg md:text-xl text-gray-600 dark:text-gray-400 mb-12 leading-relaxed max-w-3xl mx-auto animate-slide-up"
              style="animation-delay: 0.4s;">
              {{ $t('home.description') }}
            </p>

            <div class="flex flex-col sm:flex-row gap-4 justify-center mb-16 animate-slide-up"
              style="animation-delay: 0.6s;">
              <router-link to="/projects" class="btn-primary text-lg px-8 py-4 animate-pulse-slow">
                {{ $t('home.viewWork') }}
              </router-link>
              <router-link to="/contact" class="btn-secondary text-lg px-8 py-4">
                {{ $t('home.getInTouch') }}
              </router-link>
            </div>
          </div>


        </div>
      </div>
    </section>

    <!-- Quick Stats Section -->
    <section class="section-padding bg-white dark:bg-dark-800 relative overflow-hidden">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-bold mb-4 animate-slide-up">
            {{ $t('home.stats.title') }}
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('home.stats.subtitle') }}
          </p>
        </div>

        <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
          <div
            class="card  dark:bg-dark-900 p-6 text-center animate-slide-up hover:scale-105 transition-transform duration-300">
            <div class="text-4xl md:text-5xl font-bold gradient-text mb-2 animate-count">4+</div>
            <p class="text-gray-600 dark:text-gray-400">{{ $t('home.stats.experience') }}</p>
          </div>

          <div
            class="card  dark:bg-dark-900 p-6 text-center animate-slide-up hover:scale-105 transition-transform duration-300"
            style="animation-delay: 0.1s;">
            <div class="text-4xl md:text-5xl font-bold gradient-text mb-2 animate-count">15+</div>
            <p class="text-gray-600 dark:text-gray-400">{{ $t('home.stats.projects') }}</p>
          </div>

          <div
            class="card  dark:bg-dark-900 p-6 text-center animate-slide-up hover:scale-105 transition-transform duration-300"
            style="animation-delay: 0.2s;">
            <div class="text-4xl md:text-5xl font-bold gradient-text mb-2 animate-count">3</div>
            <p class="text-gray-600 dark:text-gray-400">{{ $t('home.stats.frameworks') }}</p>
          </div>

          <div
            class="card  dark:bg-dark-900 p-6 text-center animate-slide-up hover:scale-105 transition-transform duration-300"
            style="animation-delay: 0.3s;">
            <div class="text-4xl md:text-5xl font-bold gradient-text mb-2 animate-count">50%</div>
            <p class="text-gray-600 dark:text-gray-400">{{ $t('home.stats.performance') }}</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Featured Skills Section -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900 relative overflow-hidden">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-bold mb-4 animate-slide-up">
            {{ $t('home.coreTechnologies') }}
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('home.coreTechnologiesDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div class="card p-8 text-center group hover:scale-105 transition-all duration-300 animate-slide-up">
            <div
              class="w-20 h-20 mx-auto mb-6 bg-primary-100 dark:bg-primary-900 rounded-2xl flex items-center justify-center group-hover:bg-primary-200 dark:group-hover:bg-primary-800 transition-colors duration-300">

              <img
                class=" rounded-full object-cover w-10 h-10 text-primary-600 group-hover:scale-110 transition-transform duration-300"
                src="/src/assets/react.jpg" alt="react" />
            </div>
            <h3 class="text-2xl font-bold mb-4">React</h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6">Building interactive UIs with modern React patterns and
              hooks</p>

          </div>

          <div class="card p-8 text-center group hover:scale-105 transition-all duration-300 animate-slide-up"
            style="animation-delay: 0.1s;">
            <div
              class="w-20 h-20 mx-auto mb-6 bg-green-100 dark:bg-green-900 rounded-2xl flex items-center justify-center group-hover:bg-green-200 dark:group-hover:bg-green-800 transition-colors duration-300">
              <img
                class="  rounded-full object-cover w-12 h-12 text-primary-600 group-hover:scale-110 transition-transform duration-300"
                src="/src/assets/logo.svg" alt="vue" />
            </div>
            <h3 class="text-2xl font-bold mb-4">Vue.js</h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6">Creating reactive and scalable applications with Vue 3</p>

          </div>

          <div class="card p-8 text-center group hover:scale-105 transition-all duration-300 animate-slide-up"
            style="animation-delay: 0.2s;">
            <div
              class="w-20 h-20 mx-auto mb-6 bg-purple-100 dark:bg-purple-900 rounded-2xl flex items-center justify-center group-hover:bg-purple-200 dark:group-hover:bg-purple-800 transition-colors duration-300">
              <img
                class="  rounded-full object-cover w-10 h-10 text-primary-600 group-hover:scale-110 transition-transform duration-300"
                src="/src/assets/angular.png" alt="angular" />
            </div>
            <h3 class="text-2xl font-bold mb-4">Angular</h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6">Angular is a web framework that empowers developers to
              build fast, reliable applications</p>

          </div>

          <div class="card p-8 text-center group hover:scale-105 transition-all duration-300 animate-slide-up"
            style="animation-delay: 0.3s;">
            <div
              class="w-20 h-20 mx-auto mb-6 bg-red-100 dark:bg-red-900 rounded-2xl flex items-center justify-center group-hover:bg-red-200 dark:group-hover:bg-red-800 transition-colors duration-300">
              <img
                class="  rounded-full object-cover w-12 h-12 text-primary-600 group-hover:scale-110 transition-transform duration-300"
                src="/src/assets/logo-small.svg" alt="nest js" />
            </div>
            <h3 class="text-2xl font-bold mb-4">Nest.js</h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6">Server-side JavaScript for full-stack development</p>

          </div>
        </div>
      </div>
    </section>

    <!-- Articles Section -->
    <section class="section-padding bg-white dark:bg-dark-800 relative overflow-hidden">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-bold mb-4 animate-slide-up">
            {{ $t('home.articles.title') }}
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('home.articles.subtitle') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 gap-8">
          <!-- Article 1 -->
          <div class="card p-8 animate-slide-up group hover:scale-105 transition-all duration-300">
            <div class="flex items-center justify-between mb-4">
              <span
                class="px-3 py-1 bg-orange-100 dark:bg-orange-900 text-orange-700 dark:text-orange-300 rounded-full text-sm font-medium">
                {{ $t('home.articles.performance') }}
              </span>
              <span class="text-sm text-gray-500 dark:text-gray-400">Medium</span>
            </div>
            <h3
              class="text-2xl font-bold mb-4 group-hover:text-primary-600 dark:group-hover:text-primary-400 transition-colors duration-200">
              {{ $t('home.articles.article1.title') }}
            </h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
              {{ $t('home.articles.article1.description') }}
            </p>
            <div class="flex items-center justify-between">
              <div class="flex items-center space-x-2 text-sm text-gray-500 dark:text-gray-400">
                <span>📊</span>
                <span>{{ $t('home.articles.article1.readTime') }}</span>
              </div>
              <a href="https://medium.com/@sayahayoub9827/shrinking-your-spas-entry-bundle-the-key-to-faster-loads-3db155d5c6b2"
                target="_blank" rel="noopener noreferrer"
                class="inline-flex items-center text-primary-600 dark:text-primary-400 hover:text-primary-700 dark:hover:text-primary-300 transition-colors duration-200">
                {{ $t('home.articles.readMore') }}
                <svg class="w-4 h-4 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"></path>
                </svg>
              </a>
            </div>
          </div>

          <!-- Article 2 -->
          <div class="card p-8 animate-slide-up group hover:scale-105 transition-all duration-300"
            style="animation-delay: 0.1s;">
            <div class="flex items-center justify-between mb-4">
              <span
                class="px-3 py-1 bg-purple-100 dark:bg-purple-900 text-purple-700 dark:text-purple-300 rounded-full text-sm font-medium">
                {{ $t('home.articles.development') }}
              </span>
              <span class="text-sm text-gray-500 dark:text-gray-400">Medium</span>
            </div>
            <h3
              class="text-2xl font-bold mb-4 group-hover:text-primary-600 dark:group-hover:text-primary-400 transition-colors duration-200">
              {{ $t('home.articles.article2.title') }}
            </h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
              {{ $t('home.articles.article2.description') }}
            </p>
            <div class="flex items-center justify-between">
              <div class="flex items-center space-x-2 text-sm text-gray-500 dark:text-gray-400">
                <span>🧪</span>
                <span>{{ $t('home.articles.article2.readTime') }}</span>
              </div>
              <a href="https://medium.com/p/building-a-feature-catalog-with-storybook-and-msw-f9edd24324c3?source=social.linkedin&_nonce=IYKInMY8"
                target="_blank" rel="noopener noreferrer"
                class="inline-flex items-center text-primary-600 dark:text-primary-400 hover:text-primary-700 dark:hover:text-primary-300 transition-colors duration-200">
                {{ $t('home.articles.readMore') }}
                <svg class="w-4 h-4 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"></path>
                </svg>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Latest Project Preview -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900 relative overflow-hidden">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-bold mb-4 animate-slide-up">
            {{ $t('home.latestProject') }}
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('home.latestProjectDesc') }}
          </p>
        </div>

        <div class="card p-8 animate-slide-up">
          <div class="grid lg:grid-cols-2 gap-12 items-center">
            <div>
              <div class="flex items-center justify-between mb-6">
                <h3 class="text-3xl md:text-4xl font-bold">Central Bank of the Republic of Guinea</h3>
                <span
                  class="px-4 py-2 bg-green-100 dark:bg-green-900 text-green-700 dark:text-green-300 rounded-full text-sm font-medium animate-pulse">
                  {{ $t('home.current') }}
                </span>
              </div>
              <p class="text-primary-600 dark:text-primary-400 font-medium mb-4 text-lg">{{ $t('home.projectCompany') }}
                • 2025 - {{ $t('home.present') }}</p>
              <p class="text-gray-600 dark:text-gray-400 mb-8 leading-relaxed text-lg">
                {{ $t('home.projectDescription') }}
              </p>

              <div class="space-y-4 mb-8">
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-3 mr-4 flex-shrink-0 animate-pulse"></div>
                  <p class="text-gray-600 dark:text-gray-400">{{ $t('home.projectFeature1') }}</p>
                </div>
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-3 mr-4 flex-shrink-0 animate-pulse"
                    style="animation-delay: 0.5s;"></div>
                  <p class="text-gray-600 dark:text-gray-400">{{ $t('home.projectFeature2') }}</p>
                </div>
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-3 mr-4 flex-shrink-0 animate-pulse"
                    style="animation-delay: 1s;"></div>
                  <p class="text-gray-600 dark:text-gray-400">{{ $t('home.projectFeature3') }}</p>
                </div>
              </div>

              <div class="flex flex-wrap gap-3 mb-6">
                <span
                  class="px-4 py-2 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React</span>
                <span
                  class="px-4 py-2 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React
                  Query</span>
                <span
                  class="px-4 py-2 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Formio.js</span>
                <span
                  class="px-4 py-2 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">AI
                  Integration</span>
              </div>

              <router-link to="/projects" class="btn-primary inline-flex items-center">
                {{ $t('home.viewAllProjects') }}
                <svg class="w-5 h-5 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3">
                  </path>
                </svg>
              </router-link>
            </div>

            <div class="relative">
              <div
                class="bg-gradient-to-br from-green-500 to-emerald-600 rounded-2xl p-8 text-white text-center transform hover:scale-105 transition-transform duration-300">
                <div class="text-8xl font-bold mb-4 animate-bounce">🏦</div>
                <div class="text-2xl font-bold mb-2">{{ $t('home.centralBank') }}</div>
                <div class="text-lg opacity-90">{{ $t('home.guineaRepublic') }}</div>
                <div class="mt-6 text-sm opacity-75">{{ $t('home.corporateBanking') }}</div>
              </div>

              <!-- Floating elements -->
              <div class="absolute -top-4 -right-4 w-8 h-8 bg-yellow-400 rounded-full animate-float"></div>
              <div class="absolute -bottom-4 -left-4 w-6 h-6 bg-blue-400 rounded-full animate-float"
                style="animation-delay: 2s;"></div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Services Section -->
    <section class="section-padding bg-white dark:bg-dark-800 relative overflow-hidden">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-bold mb-4 animate-slide-up">
            {{ $t('home.services.title') }}
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('home.services.subtitle') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div
            class="card dark:bg-dark-900 p-8 text-center group hover:scale-105 transition-all duration-300 animate-slide-up">
            <div
              class="w-16 h-16 mx-auto mb-6 bg-primary-100 dark:bg-primary-900 rounded-2xl flex items-center justify-center group-hover:bg-primary-200 dark:group-hover:bg-primary-800 transition-colors duration-300">
              <CodeBracketIcon class="w-8 h-8 text-primary-600" />
            </div>
            <h3 class="text-2xl font-bold mb-4">{{ $t('home.services.frontend.title') }}</h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6">{{ $t('home.services.frontend.description') }}</p>
            <ul class="text-left space-y-2 text-sm text-gray-600 dark:text-gray-400">
              <li class="flex items-center">
                <div class="w-2 h-2 bg-primary-500 rounded-full mr-3"></div>
                {{ $t('home.services.frontend.feature1') }}
              </li>
              <li class="flex items-center">
                <div class="w-2 h-2 bg-primary-500 rounded-full mr-3"></div>
                {{ $t('home.services.frontend.feature2') }}
              </li>
              <li class="flex items-center">
                <div class="w-2 h-2 bg-primary-500 rounded-full mr-3"></div>
                {{ $t('home.services.frontend.feature3') }}
              </li>
            </ul>
          </div>

          <div
            class="card dark:bg-dark-900 p-8 text-center group hover:scale-105 transition-all duration-300 animate-slide-up"
            style="animation-delay: 0.1s;">
            <div
              class="w-16 h-16 mx-auto mb-6 bg-green-100 dark:bg-green-900 rounded-2xl flex items-center justify-center group-hover:bg-green-200 dark:group-hover:bg-green-800 transition-colors duration-300">
              <ServerIcon class="w-8 h-8 text-green-600" />
            </div>
            <h3 class="text-2xl font-bold mb-4">{{ $t('home.services.backend.title') }}</h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6">{{ $t('home.services.backend.description') }}</p>
            <ul class="text-left space-y-2 text-sm text-gray-600 dark:text-gray-400">
              <li class="flex items-center">
                <div class="w-2 h-2 bg-green-500 rounded-full mr-3"></div>
                {{ $t('home.services.backend.feature1') }}
              </li>
              <li class="flex items-center">
                <div class="w-2 h-2 bg-green-500 rounded-full mr-3"></div>
                {{ $t('home.services.backend.feature2') }}
              </li>
              <li class="flex items-center">
                <div class="w-2 h-2 bg-green-500 rounded-full mr-3"></div>
                {{ $t('home.services.backend.feature3') }}
              </li>
            </ul>
          </div>

          <div
            class="card dark:bg-dark-900 p-8 text-center group hover:scale-105 transition-all duration-300 animate-slide-up"
            style="animation-delay: 0.2s;">
            <div
              class="w-16 h-16 mx-auto mb-6 bg-purple-100 dark:bg-purple-900 rounded-2xl flex items-center justify-center group-hover:bg-purple-200 dark:group-hover:bg-purple-800 transition-colors duration-300">
              <CogIcon class="w-8 h-8 text-purple-600" />
            </div>
            <h3 class="text-2xl font-bold mb-4">{{ $t('home.services.consulting.title') }}</h3>
            <p class="text-gray-600 dark:text-gray-400 mb-6">{{ $t('home.services.consulting.description') }}</p>
            <ul class="text-left space-y-2 text-sm text-gray-600 dark:text-gray-400">
              <li class="flex items-center">
                <div class="w-2 h-2 bg-purple-500 rounded-full mr-3"></div>
                {{ $t('home.services.consulting.feature1') }}
              </li>
              <li class="flex items-center">
                <div class="w-2 h-2 bg-purple-500 rounded-full mr-3"></div>
                {{ $t('home.services.consulting.feature2') }}
              </li>
              <li class="flex items-center">
                <div class="w-2 h-2 bg-purple-500 rounded-full mr-3"></div>
                {{ $t('home.services.consulting.feature3') }}
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- Call to Action Section -->
    <section class="section-padding bg-gradient-to-r from-primary-600 to-purple-600 relative overflow-hidden">
      <div class="container-custom">
        <div class="text-center text-white">
          <h2 class="text-4xl md:text-5xl font-bold mb-6 animate-slide-up">
            {{ $t('home.cta.title') }}
          </h2>
          <p class="text-xl mb-8 opacity-90 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('home.cta.description') }}
          </p>
          <div class="flex flex-col sm:flex-row gap-4 justify-center animate-slide-up" style="animation-delay: 0.4s;">
            <router-link to="/contact"
              class="bg-white text-primary-600 px-8 py-4 rounded-lg font-semibold hover:bg-gray-100 transition-colors duration-200 text-lg">
              {{ $t('home.cta.primaryButton') }}
            </router-link>
            <router-link to="/projects"
              class="border-2 border-white text-white px-8 py-4 rounded-lg font-semibold hover:bg-white hover:text-primary-600 transition-colors duration-200 text-lg">
              {{ $t('home.cta.secondaryButton') }}
            </router-link>
          </div>
        </div>
      </div>

      <!-- Floating elements -->
      <div class="absolute top-10 left-10 w-4 h-4 bg-white rounded-full opacity-20 animate-float"></div>
      <div class="absolute top-20 right-20 w-6 h-6 bg-white rounded-full opacity-20 animate-float"
        style="animation-delay: 1s;"></div>
      <div class="absolute bottom-10 left-1/4 w-3 h-3 bg-white rounded-full opacity-20 animate-float"
        style="animation-delay: 2s;"></div>
      <div class="absolute bottom-20 right-1/4 w-5 h-5 bg-white rounded-full opacity-20 animate-float"
        style="animation-delay: 3s;"></div>
    </section>
  </div>
</template>

<style scoped>
.typing-text {
  position: relative;
  display: inline-block;
}

.typing-text::after {
  content: '';
  position: absolute;
  right: -4px;
  top: 0;
  height: 100%;
  width: 3px;
  background: #3b82f6;
  animation: blink-caret 0.75s step-end infinite;
}

@keyframes blink-caret {

  from,
  to {
    opacity: 0;
  }

  50% {
    opacity: 1;
  }
}

/* Add a subtle fade-in effect for the text */
.typing-text {
  animation: fadeInText 2s ease-in-out;
}

@keyframes fadeInText {
  0% {
    opacity: 0;
    transform: translateY(10px);
  }

  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
