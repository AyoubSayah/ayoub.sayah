<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section
      class="relative min-h-screen flex items-center justify-center overflow-hidden bg-gradient-to-br from-primary-50 via-white to-purple-50 dark:from-dark-900 dark:via-dark-800 dark:to-dark-900">
      <canvas ref="threeCanvas" class="absolute inset-0 z-0"></canvas>

      <!-- Floating JS Ecosystem Logos -->
      <div class="absolute inset-0 overflow-hidden z-[20]">
        <img src="../assets/angular.png" class="absolute rounded-full top-10 left-16 w-16 opacity-80 animate-float-slow"
          alt="JavaScript" />
        <img src="../assets/vue.png"
          class="absolute rounded-full top-1/2 left-10 w-16 h-16 object-cover opacity-80 animate-float" alt="React" />
        <img src="../assets/typescript.png" class="absolute rounded-full top-1/3 right-20 w-14 opacity-80 animate-float"
          alt="Vue" />
        <img src="../assets/logo-small.svg"
          class="absolute rounded-full bottom-20 left-1/4 w-14 opacity-80 animate-float" alt="Angular" />
        <img src="../assets/react.jpg"
          class="absolute rounded-full bottom-10  object-cover w-14 h-14 right-16 opacity-80 animate-float-slow"
          alt="Node.js" />
      </div>
      <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
        <svg class="w-10 h-10 text-purple-600" fill="currentColor" viewBox="0 0 24 24">
          <path d="M12 16l-6-6h12z" />
        </svg>
      </div>

      <!-- Animated Background Blobs -->
      <div class="absolute inset-0 overflow-hidden z-10">
        <div
          class="absolute top-20 z-10 left-20 w-72 h-72 bg-primary-300 dark:bg-primary-700 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-float">
        </div>
        <div
          class="absolute top-40 z-10 right-20 w-96 h-96 bg-purple-300 dark:bg-purple-700 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-float"
          style="animation-delay: 2s;"></div>
        <div
          class="absolute bottom-20 z-10 left-1/2 w-80 h-80 bg-pink-300 dark:bg-pink-700 rounded-full mix-blend-multiply filter blur-xl opacity-20 animate-float"
          style="animation-delay: 4s;"></div>
      </div>

      <!-- Content -->
      <div class="container-custom relative z-10">
        <div class="max-w-4xl mx-auto text-center">
          <div class="animate-bounce-in">
            <p class="text-xl md:text-3xl text-primary-600 dark:text-primary-400 mb-4 animate-slide-down">
              {{ $t('home.greeting') }}
            </p>
            <h1 class="text-5xl md:text-5xl lg:text-7xl font-bold mb-6 animate-slide-up">
              <span class="gradient-text">Ayoub Sayah</span>
            </h1>
            <h2
              class="text-2xl md:text-3xl lg:text-2xl font-semibold mb-8 text-gray-700 dark:text-gray-300 animate-slide-up"
              style="animation-delay: 0.2s;">
              <span>{{ $t('home.title') }}</span>
            </h2>
            <div class="min-h-[10rem] ">
              <p ref="description"
                class="text-lg min-h-[8rem] inline-block md:text-xl text-gray-600 dark:text-gray-400 mb-12 leading-relaxed max-w-3xl mx-auto animate-slide-up"
                style="animation-delay: 0.4s;">
                <!-- {{ $t('home.description') }} -->
              </p>
            </div>
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
            <div class="text-4xl md:text-5xl font-bold gradient-text mb-2 animate-count">5+</div>
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
    <Certification />

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
          <div class="card  dark:bg-dark-900  p-8 animate-slide-up group hover:scale-105 transition-all duration-300">
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
          <div class="card  dark:bg-dark-900  p-8 animate-slide-up group hover:scale-105 transition-all duration-300"
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
          <div class="flex flex-col sm:flex-row gap-4 justify-center animate-slide-up mt-4"
            style="animation-delay: 0.4s;">
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
<script lang="ts" setup>
import {
  CodeBracketIcon,
  ServerIcon,
  CogIcon
} from '@heroicons/vue/24/outline'
import Certification from '../components/Certfication.vue'
import { useTemplateRef, watchEffect } from 'vue';
import { onMounted } from 'vue';
import Typed from 'typed.js';
import { useI18n } from 'vue-i18n';
import * as THREE from 'three';
const { t, } = useI18n();
const description = useTemplateRef("description")
const threeCanvas = useTemplateRef("threeCanvas");
import tsLogo from '@/assets/typescript.png';
import jsLogo from '@/assets/logo-small.svg';
import vueLogo from '@/assets/vue.png';
import reactLogo from '@/assets/react.svg';
import angularLogo from '@/assets/angular.png';
import storybookLogo from '@/assets/storybook.webp';
let descriptionTypedInstance: Typed | null = null;

watchEffect(async () => {
  const text = t("home.description");
  descriptionTypedInstance?.destroy();

  if (description?.value) {
    descriptionTypedInstance = new Typed(description.value, {
      strings: [text],
      typeSpeed: 60,
      backSpeed: 40,
      loop: true,
      smartBackspace: true,
      backDelay: 1500,
    });// Adjust typing speed here
  }
});
onMounted(() => {
  initThreeJS();
});
const initThreeJS = () => {
  if (!threeCanvas?.value) return;
  const scene = new THREE.Scene();
  const camera = new THREE.PerspectiveCamera(50, window.innerWidth / window.innerHeight, 0.1, 1000);
  camera.position.z = 5;

  const renderer = new THREE.WebGLRenderer({ canvas: threeCanvas.value, alpha: true });
  renderer.setSize(window.innerWidth, window.innerHeight);

  // Light
  const light = new THREE.AmbientLight(0xffffff, 1);
  scene.add(light);

  // Orbiting JS logos (as spheres with textures)
  const loader = new THREE.TextureLoader();
  const logos = [
    tsLogo,
    jsLogo,
    vueLogo,
    reactLogo,
    angularLogo,
    storybookLogo
  ];

  const spheres = logos.map((src, i) => {
    const geometry = new THREE.CylinderGeometry(0.5, 0.5, 0.05, 64); // radiusTop, radiusBottom, height, segments
    const material = new THREE.MeshStandardMaterial({
      map: loader.load(src),
      metalness: 0.4,
      roughness: 0.7,

    });
    const ambient = new THREE.AmbientLight(0xffffff, 0.6); // soft fill
    scene.add(ambient);

    const directional = new THREE.DirectionalLight(0xffffff, 0.6);
    directional.position.set(5, 5, 5);
    scene.add(directional);
    const sphere = new THREE.Mesh(geometry, material);
    sphere.position.set(Math.cos(i * Math.PI) * 2, Math.sin(i * Math.PI) * 1.5, 0);

    scene.add(sphere);

    return sphere;
  });

  // Animation
  const animate = () => {
    requestAnimationFrame(animate);
    spheres.forEach((s, i) => {
      s.rotation.x += 0.005;
      s.rotation.y += 0.01;
      s.position.x = Math.cos(Date.now() * 0.001 + i) * 2;
      s.position.y = Math.sin(Date.now() * 0.001 + i) * 1.5;
      s.position.z = Math.sin(Date.now() * 0.001 + i) * 0.5; // gives depth
    });
    renderer.render(scene, camera);
  };

  animate();

  window.addEventListener("resize", () => {
    camera.aspect = window.innerWidth / window.innerHeight;
    camera.updateProjectionMatrix();
    renderer.setSize(window.innerWidth, window.innerHeight);
  });
};
</script>
<style>
.typing-text {
  position: relative;
  display: inline-block;
}

.typed-cursor {
  display: inline-block;
  vertical-align: middle;
  /* Keep cursor aligned with text */
  font-weight: bold;
  color: #6b46c1;
  /* or your theme color */
}

p {
  display: inline;
  /* Matches text */
  vertical-align: middle;
}

img:hover {
  transform: scale(1.1) rotate(5deg);
  transition: transform 0.3s ease;
  filter: drop-shadow(0 0 10px #6b46c1);
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
