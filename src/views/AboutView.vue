<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section
      class="section-padding bg-gradient-to-br from-primary-50 via-white to-purple-50 dark:from-dark-900 dark:via-dark-800 dark:to-dark-900">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto text-center">
          <h1 class="text-5xl md:text-6xl font-bold mb-6 animate-slide-up">
            {{ $t('about.title') }}
          </h1>
          <p class="text-xl text-gray-600 dark:text-gray-400 mb-8 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('about.subtitle') }}
          </p>
        </div>
      </div>
    </section>

    <!-- About Me Section -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto">
          <div class="grid lg:grid-cols-2 gap-12 items-center">
            <div class="animate-slide-left">
              <h2 class="text-3xl font-bold mb-6">{{ $t('about.whoIAm') }}</h2>
              <div class="space-y-6 text-lg text-gray-600 dark:text-gray-400 leading-relaxed">
                <p>{{ $t('about.description1') }}</p>
                <p>{{ $t('about.description2') }}</p>
                <p>{{ $t('about.description3') }}</p>
              </div>
            </div>

            <div class="animate-slide-right">
              <div class="card p-8 dark:bg-dark-900">
                <h3 class="text-2xl font-bold mb-6">{{ $t('about.personalInfo') }}</h3>
                <div class="space-y-4">
                  <div class="flex items-center">
                    <div class="w-3 h-3 bg-primary-500 rounded-full mr-4"></div>
                    <span class="font-medium">Name:</span>
                    <span class="ml-2">Ayoub Sayah</span>
                  </div>
                  <div class="flex items-center">
                    <div class="w-3 h-3 bg-primary-500 rounded-full mr-4"></div>
                    <span class="font-medium">Location:</span>
                    <span class="ml-2">Sousse, Tunisia</span>
                  </div>
                  <div class="flex items-center">
                    <div class="w-3 h-3 bg-primary-500 rounded-full mr-4"></div>
                    <span class="font-medium">Experience:</span>
                    <span class="ml-2">5+ Years</span>
                  </div>
                  <div class="flex items-center">
                    <div class="w-3 h-3 bg-primary-500 rounded-full mr-4"></div>
                    <span class="font-medium">Specialization:</span>
                    <span class="ml-2">Frontend Development</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Education Section -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('about.education') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('about.educationDesc') }}
          </p>
        </div>

        <div class="max-w-4xl mx-auto">
          <div class="card p-8 animate-slide-up mb-8">
            <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-6">
              <div>
                <h3 class="text-2xl font-bold mb-2">Engineering Degree in Computer Engineering</h3>
                <p class="text-xl text-primary-600 dark:text-primary-400 mb-2">
                  EPI Sousse University
                </p>
                <p class="text-gray-600 dark:text-gray-400">Sousse, Tunisia</p>
              </div>
              <div class="mt-4 md:mt-0">
                <span
                  class="px-4 py-2 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">
                  2021 - 2025
                </span>
              </div>
            </div>

            <div class="space-y-4">
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Focused on algorithms, system design, and artificial intelligence techniques
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Developed AI models and machine learning applications using Python, TensorFlow, and PyTorch
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Acquired skills in Power BI, data visualization, and business intelligence
                </p>
              </div>
            </div>
          </div>
          <div class="card p-8 animate-slide-up">
            <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-6">
              <div>
                <h3 class="text-2xl font-bold mb-2">Bachelor's Degree in Computer Management</h3>
                <p class="text-xl text-primary-600 dark:text-primary-400 mb-2"> Higher Institute of Management of Sousse
                </p>
                <p class="text-gray-600 dark:text-gray-400">Sousse, Tunisia</p>
              </div>
              <div class="mt-4 md:mt-0">
                <span
                  class="px-4 py-2 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">
                  2017 - 2021
                </span>
              </div>
            </div>

            <div class="space-y-4">
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Specialized in software engineering and web development
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Completed projects in React, Vue.js, and full-stack development
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Graduated with honors and strong academic performance
                </p>
              </div>
            </div>
          </div>


        </div>
      </div>
    </section>

    <!-- Languages Section -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('about.languages') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('about.languagesDesc') }}
          </p>
        </div>

        <div class="max-w-4xl mx-auto">
          <div class="grid md:grid-cols-3 gap-8">
            <div class="card p-6 text-center animate-slide-up">
              <div class="text-4xl mb-4">🇫🇷</div>
              <h3 class="text-xl font-bold mb-2">French</h3>
              <p class="text-gray-600 dark:text-gray-400 mb-4">Professional</p>
              <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2">
                <div class="bg-primary-600 h-2 rounded-full" style="width: 90%"></div>
              </div>
            </div>

            <div class="card p-6 text-center animate-slide-up" style="animation-delay: 0.1s;">
              <div class="text-4xl mb-4">EN</div>
              <h3 class="text-xl font-bold mb-2">English</h3>
              <p class="text-gray-600 dark:text-gray-400 mb-4">Professional</p>
              <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2">
                <div class="bg-primary-600 h-2 rounded-full" style="width: 90%"></div>
              </div>
            </div>

            <div class="card p-6 text-center animate-slide-up" style="animation-delay: 0.2s;">
              <div class="text-4xl mb-4">🇹🇳</div>
              <h3 class="text-xl font-bold mb-2">Arabic</h3>
              <p class="text-gray-600 dark:text-gray-400 mb-4">Native</p>
              <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2">
                <div class="bg-primary-600 h-2 rounded-full" style="width: 100%"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Certifications Section -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('about.certifications') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('about.certificationsDesc') }}
          </p>
        </div>

        <div class="max-w-4xl mx-auto">
          <div class="grid md:grid-cols-2 gap-8">
            <div class="card p-6 animate-slide-up">
              <div class="flex items-start">
                <div
                  class="w-12 h-12 bg-primary-100 dark:bg-primary-900 rounded-lg flex items-center justify-center mr-4 flex-shrink-0">
                  <svg class="w-6 h-6 text-primary-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg font-bold mb-2">Angular Developer Certification</h3>
                  <p class="text-primary-600 dark:text-primary-400 text-sm mb-2">Certficates.dev</p>
                  <p class="text-gray-600 dark:text-gray-400 text-sm">Advanced Angular concepts and best practices</p>
                </div>
              </div>
            </div>

            <div class="card p-6 animate-slide-up" style="animation-delay: 0.1s;">
              <div class="flex items-start">
                <div
                  class="w-12 h-12 bg-green-100 dark:bg-green-900 rounded-lg flex items-center justify-center mr-4 flex-shrink-0">
                  <svg class="w-6 h-6 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg font-bold mb-2">Vue.js Developer Certification</h3>
                  <p class="text-green-600 dark:text-green-400 text-sm mb-2">Certficates.dev</p>
                  <p class="text-gray-600 dark:text-gray-400 text-sm">Vue 3 Composition API and ecosystem</p>
                </div>
              </div>
            </div>

            <div class="card p-6 animate-slide-up" style="animation-delay: 0.2s;">
              <div class="flex items-start">
                <div
                  class="w-12 h-12 bg-purple-100 dark:bg-purple-900 rounded-lg flex items-center justify-center mr-4 flex-shrink-0">
                  <svg class="w-6 h-6 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg font-bold mb-2">Cloud Practitioner</h3>
                  <p class="text-purple-600 dark:text-purple-400 text-sm mb-2">Aws</p>
                  <p class="text-gray-600 dark:text-gray-400 text-sm">Aws certified cloud practitioner</p>
                </div>
              </div>
            </div>

            <div class="card p-6 animate-slide-up" style="animation-delay: 0.3s;">
              <div class="flex items-start">
                <div
                  class="w-12 h-12 bg-blue-100 dark:bg-blue-900 rounded-lg flex items-center justify-center mr-4 flex-shrink-0">
                  <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg font-bold mb-2">JavaScript algorithms Certification</h3>
                  <p class="text-blue-600 dark:text-blue-400 text-sm mb-2">FreecodeCamp</p>
                  <p class="text-gray-600 dark:text-gray-400 text-sm">JavaScript and APIs</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
// No additional script needed for this view
</script>
