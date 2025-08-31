<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section
      class="section-padding bg-gradient-to-br from-primary-50 via-white to-purple-50 dark:from-dark-900 dark:via-dark-800 dark:to-dark-900">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto text-center">
          <h1 class="text-5xl md:text-6xl font-bold mb-6 animate-slide-up">
            {{ $t('experience.title') }}
          </h1>
          <p class="text-xl text-gray-600 dark:text-gray-400 mb-8 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('experience.subtitle') }}
          </p>
        </div>
      </div>
    </section>

    <!-- Current Role -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto">
          <div class="card p-8 animate-slide-up dark:bg-dark-900">
            <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-6">
              <div>
                <h2 class="text-3xl font-bold mb-2">Frontend Developer</h2>
                <p class="text-xl text-primary-600 dark:text-primary-400 mb-2">Proxym-IT</p>
                <p class="text-gray-600 dark:text-gray-400">Sousse, Tunisia</p>
              </div>
              <div class="mt-4 md:mt-0">
                <span
                  class="px-4 py-2 bg-green-100 dark:bg-green-900 text-green-700 dark:text-green-300 rounded-full text-sm font-medium">
                  September 2021 - Present
                </span>
              </div>
            </div>

            <div class="space-y-4 mb-6">
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Developed banking interfaces for over 10,000 users using React, TypeScript, and Chakra UI
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Migrated state management to React Query, reducing boilerplate by 30% and API calls by 25%
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Optimized bundle size by 50% using code splitting for faster load times
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Created forms using Formio.js, a low-code platform, simplifying user onboarding processes
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Implemented unit testing with Jest, reducing development bugs by over 40%
                </p>
              </div>
              <div class="flex items-start">
                <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                <p class="text-gray-600 dark:text-gray-400">
                  Implemented Storybook and Cypress for UI and end-to-end testing, reducing production bugs by 30%
                </p>
              </div>
            </div>

            <div class="flex flex-wrap gap-2">
              <span
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React</span>
              <span
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">TypeScript</span>
              <span
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Chakra
                UI</span>
              <span
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React
                Query</span>
              <span
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Jest</span>
              <span
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Cypress</span>
              <span
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Storybook</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Previous Experience -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto">
          <h2 class="text-3xl font-bold mb-12 text-center animate-slide-up">{{ $t('experience.previousExperience') }}
          </h2>

          <div class="space-y-8">
            <!-- Junior Frontend Developer -->
            <div class="card p-8 animate-slide-up" style="animation-delay: 0.1s;">
              <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-6">
                <div>
                  <h3 class="text-2xl font-bold mb-2">Junior Frontend Developer</h3>
                  <p class="text-xl text-primary-600 dark:text-primary-400 mb-2">Alfaprint</p>
                  <p class="text-gray-600 dark:text-gray-400">Sousse, Tunisia</p>
                </div>
                <div class="mt-4 md:mt-0">
                  <span
                    class="px-4 py-2 bg-gray-100 dark:bg-gray-700 text-gray-700 dark:text-gray-300 rounded-full text-sm font-medium">
                    April 2021 - September 2021
                  </span>
                </div>
              </div>

              <div class="space-y-4 mb-6">
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                  <p class="text-gray-600 dark:text-gray-400">
                    Built an SEO-optimized e-commerce platform using React and Bootstrap
                  </p>
                </div>
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                  <p class="text-gray-600 dark:text-gray-400">
                    Achieved a 99% Google PageSpeed score through advanced optimization techniques
                  </p>
                </div>
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                  <p class="text-gray-600 dark:text-gray-400">
                    Increased organic traffic by 40% and conversion rates by 25%
                  </p>
                </div>
              </div>

              <div class="flex flex-wrap gap-2">
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React</span>
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Bootstrap</span>
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">SEO</span>
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Performance</span>
              </div>
            </div>

            <!-- Full-Stack Developer Intern -->
            <div class="card p-8 animate-slide-up" style="animation-delay: 0.2s;">
              <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-6">
                <div>
                  <h3 class="text-2xl font-bold mb-2">Full-Stack Developer Intern</h3>
                  <p class="text-xl text-primary-600 dark:text-primary-400 mb-2">Children's Club Platform</p>
                  <p class="text-gray-600 dark:text-gray-400">Sousse, Tunisia</p>
                </div>
                <div class="mt-4 md:mt-0">
                  <span
                    class="px-4 py-2 bg-gray-100 dark:bg-gray-700 text-gray-700 dark:text-gray-300 rounded-full text-sm font-medium">
                    February 2020 - September 2020
                  </span>
                </div>
              </div>

              <div class="space-y-4 mb-6">
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                  <p class="text-gray-600 dark:text-gray-400">
                    Developed a full-stack platform using Angular, Express.js, and MongoDB
                  </p>
                </div>
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                  <p class="text-gray-600 dark:text-gray-400">
                    Implemented user management, activity scheduling, and parent communication features
                  </p>
                </div>
                <div class="flex items-start">
                  <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                  <p class="text-gray-600 dark:text-gray-400">
                    Implemented responsive design and real-time notifications using Socket.IO
                  </p>
                </div>
              </div>

              <div class="flex flex-wrap gap-2">
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Angular</span>
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Express.js</span>
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">MongoDB</span>
                <span
                  class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Socket.IO</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Key Achievements -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('experience.keyAchievements') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('experience.keyAchievementsDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div class="card dark:bg-dark-900 p-6 text-center animate-slide-up">
            <div class="text-4xl font-bold gradient-text mb-2">10K+</div>
            <p class="text-gray-600 dark:text-gray-400">Users Served</p>
          </div>

          <div class="card dark:bg-dark-900 p-6 text-center animate-slide-up" style="animation-delay: 0.1s;">
            <div class="text-4xl font-bold gradient-text mb-2">50%</div>
            <p class="text-gray-600 dark:text-gray-400">Bundle Size Reduction</p>
          </div>

          <div class="card dark:bg-dark-900 p-6 text-center animate-slide-up" style="animation-delay: 0.2s;">
            <div class="text-4xl font-bold gradient-text mb-2">40%</div>
            <p class="text-gray-600 dark:text-gray-400">Bug Reduction</p>
          </div>

          <div class="card dark:bg-dark-900 p-6 text-center animate-slide-up" style="animation-delay: 0.3s;">
            <div class="text-4xl font-bold gradient-text mb-2">99%</div>
            <p class="text-gray-600 dark:text-gray-400">PageSpeed Score</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
// No additional script needed for this view
</script>
