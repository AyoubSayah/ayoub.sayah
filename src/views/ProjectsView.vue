<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section
      class="section-padding bg-gradient-to-br from-primary-50 via-white to-purple-50 dark:from-dark-900 dark:via-dark-800 dark:to-dark-900">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto text-center">
          <h1 class="text-5xl md:text-6xl font-bold mb-6 animate-slide-up">
            {{ $t('projects.title') }}
          </h1>
          <p class="text-xl text-gray-600 dark:text-gray-400 mb-8 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('projects.subtitle') }}
          </p>
        </div>
      </div>
    </section>

    <!-- Featured Projects -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('projects.featuredProjects') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('projects.featuredProjectsDesc') }}
          </p>
        </div>

        <div class="space-y-12">
          <!-- Banque Centrale de la République de Guinée -->
          <div class="card dark:bg-dark-900 p-8 animate-slide-up">
            <div class="grid lg:grid-cols-2 gap-8 items-center">
              <div>
                <div class="flex items-center justify-between mb-4">
                  <h3 class="text-3xl font-bold">Central Bank of the Republic of Guinea</h3>
                  <span
                    class="px-3 py-1 bg-green-100 dark:bg-green-900 text-green-700 dark:text-green-300 rounded-full text-sm font-medium">
                    Current
                  </span>
                </div>
                <p class="text-primary-600 dark:text-primary-400 font-medium mb-4">Proxym-IT • 2025 - Present</p>
                <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                  Developed a comprehensive corporate banking platform for the Central Bank of Guinea.
                  Implemented advanced React Query integration with Formio.js, including custom fetch function overrides
                  and AI-powered form generation capabilities.
                </p>
                <div class="space-y-3 mb-6">
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Built corporate banking interfaces using React and React
                      Query</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Overrode Formio.js fetch function to integrate with
                      React Query</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Implemented AI-powered form generation using Formio.js
                    </p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Enhanced data management and caching with React Query
                    </p>
                  </div>
                </div>
                <div class="flex flex-wrap gap-2 mb-6">
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React
                    Query</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Formio.js</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">AI
                    Integration</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Corporate
                    Banking</span>
                </div>
                <div class="text-sm text-gray-500 dark:text-gray-400">
                  <strong>Type:</strong> Central Bank Platform
                </div>
              </div>
              <div class="bg-gradient-to-br from-green-500 to-emerald-600 rounded-lg p-8 text-white text-center">
                <div class="text-6xl font-bold mb-2">🏦</div>
                <div class="text-lg mb-4">Central Bank</div>
                <div class="text-sm opacity-90">Guinea Republic</div>
              </div>
            </div>
          </div>

          <!-- Wingman Project -->
          <div class="card dark:bg-dark-900 p-8 animate-slide-up" style="animation-delay: 0.1s;">
            <div class="grid lg:grid-cols-2 gap-8 items-center">
              <div>
                <div class="flex items-center justify-between mb-4">
                  <h3 class="text-3xl font-bold">Wingman</h3>
                  <span
                    class="px-3 py-1 bg-blue-100 dark:bg-blue-900 text-blue-700 dark:text-blue-300 rounded-full text-sm font-medium">
                    Completed
                  </span>
                </div>
                <p class="text-primary-600 dark:text-primary-400 font-medium mb-4">Freelance • 2025</p>
                <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                  Designed and implemented a full-stack application architecture using Next.js and NestJS.
                  Created a modern tech stack with Tailwind CSS, Hero UI, React Query, and Zustand for state management.
                </p>
                <div class="space-y-3 mb-6">
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Architected full-stack solution with Next.js frontend
                      and NestJS backend</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Implemented modern frontend with Tailwind CSS and Hero
                      UI components</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Used React Query for server state management and Zustand
                      for client state</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Backend built with TypeORM and PostgreSQL for robust
                      data management</p>
                  </div>
                </div>
                <div class="flex flex-wrap gap-2 mb-6">
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Next.js</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">NestJS</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Tailwind
                    CSS</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React
                    Query</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Zustand</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">TypeORM</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">PostgreSQL</span>
                </div>
                <div class="text-sm text-gray-500 dark:text-gray-400">
                  <strong>Type:</strong> Full-Stack Application
                </div>
              </div>
              <div class="bg-gradient-to-br from-blue-500 to-cyan-600 rounded-lg p-8 text-white text-center">
                <div class="text-6xl font-bold mb-2">🚀</div>
                <div class="text-lg mb-4">Full-Stack</div>
                <div class="text-sm opacity-90">Modern Architecture</div>
              </div>
            </div>
          </div>

          <!-- FAB Project -->
          <div class="card dark:bg-dark-900 p-8 animate-slide-up" style="animation-delay: 0.2s;">
            <div class="grid lg:grid-cols-2 gap-8 items-center">
              <div>
                <div class="flex items-center justify-between mb-4">
                  <h3 class="text-3xl font-bold">First Abu Dhabi Bank Misr Platform</h3>
                  <span
                    class="px-3 py-1 bg-green-100 dark:bg-green-900 text-green-700 dark:text-green-300 rounded-full text-sm font-medium">
                    Current
                  </span>
                </div>
                <p class="text-primary-600 dark:text-primary-400 font-medium mb-4">Proxym-IT • August 2024 - Present</p>
                <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                  Developed a comprehensive microloan and savings platform serving 10,000+ users. Streamlined user flows
                  with dynamic loan application forms using Formio, and collaborated with backend and BI teams for
                  accurate financial reporting.
                </p>
                <div class="space-y-3 mb-6">
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Built responsive banking interfaces using React, Chakra
                      UI, and Redux</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Designed dynamic loan application forms with Formio for
                      improved usability</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Worked in Agile environment with regular sprints and
                      close collaboration</p>
                  </div>
                </div>
                <div class="flex flex-wrap gap-2 mb-6">
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Chakra
                    UI</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Redux</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Formio</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Agile</span>
                </div>
                <div class="text-sm text-gray-500 dark:text-gray-400">
                  <strong>Team:</strong> 8 Frontend, 5 Backend, 1 PO, 1 PM
                </div>
              </div>
              <div class="bg-gradient-to-br from-primary-500 to-purple-600 rounded-lg p-8 text-white text-center">
                <div class="text-6xl font-bold mb-2">10K+</div>
                <div class="text-lg mb-4">Active Users</div>
                <div class="text-sm opacity-90">Microfinance Platform</div>
              </div>
            </div>
          </div>

          <!-- Bankerise Corporate -->
          <div class="card dark:bg-dark-900 p-8 animate-slide-up" style="animation-delay: 0.3s;">
            <div class="grid lg:grid-cols-2 gap-8 items-center">
              <div>
                <div class="flex items-center justify-between mb-4">
                  <h3 class="text-3xl font-bold">Bankerise Corporate</h3>
                  <span
                    class="px-3 py-1 bg-blue-100 dark:bg-blue-900 text-blue-700 dark:text-blue-300 rounded-full text-sm font-medium">
                    Completed
                  </span>
                </div>
                <p class="text-primary-600 dark:text-primary-400 font-medium mb-4">Proxym-IT • July 2023 - May 2024</p>
                <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                  Built enterprise banking solution for 50+ corporate clients with 50% performance improvement.
                  Migrated state management to React Query, optimized bundle size, and implemented comprehensive
                  testing.
                </p>
                <div class="space-y-3 mb-6">
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Built responsive banking interfaces using React and
                      Chakra UI</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Migrated state management to React Query, reducing
                      boilerplate by 30%</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Optimized bundle size by 50% for faster load times</p>
                  </div>
                </div>
                <div class="flex flex-wrap gap-2 mb-6">
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">TypeScript</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">React
                    Query</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Storybook</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Cypress</span>
                </div>
                <div class="text-sm text-gray-500 dark:text-gray-400">
                  <strong>Team:</strong> 3 Frontend, 4 Backend, 2 DevOps, 1 PO, 1 PM, 2 BI
                </div>
              </div>
              <div class="bg-gradient-to-br from-blue-500 to-cyan-600 rounded-lg p-8 text-white text-center">
                <div class="text-6xl font-bold mb-2">5+</div>
                <div class="text-lg mb-4">Corporate Clients</div>
                <div class="text-sm opacity-90">Enterprise Banking</div>
              </div>
            </div>
          </div>
          <div class="card dark:bg-dark-900 p-8 animate-slide-up" style="animation-delay: 0.3s;">
            <div class="grid lg:grid-cols-2 gap-8 items-center">
              <div>
                <div class="flex items-center justify-between mb-4">
                  <h3 class="text-3xl font-bold">E-Commerce Web App</h3>
                  <span
                    class="px-3 py-1 bg-green-100 dark:bg-green-900 text-green-700 dark:text-green-300 rounded-full text-sm font-medium">
                    Portfolio
                  </span>
                </div>
                <p class="text-primary-600 dark:text-primary-400 font-medium mb-4">Personal Project • 2025</p>
                <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                  Developed a fully responsive e-commerce application showcasing <strong>multi-theming</strong> and
                  <strong>smooth animations</strong> to highlight UI/UX skills. Integrated Firebase for authentication,
                  Firestore for product storage, and optimized performance with lazy loading and image compression.
                </p>
                <div class="space-y-3 mb-6">
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Implemented light, dark, and custom themes with instant
                      switching</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Designed smooth page transitions and interactive cart
                      animations</p>
                  </div>
                  <div class="flex items-start">
                    <div class="w-2 h-2 bg-primary-500 rounded-full mt-2 mr-4 flex-shrink-0"></div>
                    <p class="text-gray-600 dark:text-gray-400">Built shopping cart and checkout flow with Firebase Auth
                      & Firestore</p>
                  </div>
                </div>
                <div class="flex flex-wrap gap-2 mb-6">
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Vue</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">TailwindCSS</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Pinia</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Firebase</span>
                  <span
                    class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">Animations</span>
                </div>
                <div class="text-sm text-gray-500 dark:text-gray-400">
                  <strong>Links:</strong>
                  <a href="https://ecommerce-261605.web.app" target="_blank" class="underline">Live Demo</a> •
                  <a href="https://github.com/AyoubSayah/templateEcommerceVue" target="_blank"
                    class="underline">GitHub</a>
                </div>
              </div>
              <div class="bg-gradient-to-br from-green-500 to-emerald-600 rounded-lg p-8 text-white text-center">
                <div class="text-6xl font-bold mb-2">✨</div>
                <div class="text-lg mb-4">Multi-Theming</div>
                <div class="text-sm opacity-90">Animations & UI Craftsmanship</div>
              </div>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- Other Projects -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('projects.otherProjects') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('projects.otherProjectsDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- CSA Legacy Migration -->
          <div class="card dark:bg-dark-900 p-6 animate-slide-up">
            <h3 class="text-xl font-bold mb-2">CSA Legacy Migration</h3>
            <p class="text-primary-600 dark:text-primary-400 text-sm mb-3">Proxym-IT • February 2023 - June 2023</p>
            <p class="text-gray-600 dark:text-gray-400 mb-4">
              Successfully migrated a legacy JSF dashboard to React, reducing load times by 45% and
              rebuilding core modules with Redux and Formio for better maintainability.
            </p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">React</span>
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">TypeScript</span>
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">Redux</span>
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">Formio</span>
            </div>
            <div class="text-xs text-gray-500 dark:text-gray-400">
              <strong>Achievement:</strong> 45% Load Time Reduction
            </div>
          </div>

          <!-- Bankerise -->
          <div class="card dark:bg-dark-900 p-6 animate-slide-up" style="animation-delay: 0.1s;">
            <h3 class="text-xl font-bold mb-2">Bankerise</h3>
            <p class="text-primary-600 dark:text-primary-400 text-sm mb-3">Proxym-IT • September 2021 - January 2022</p>
            <p class="text-gray-600 dark:text-gray-400 mb-4">
              Contributed to an omnichannel banking platform using React and Redux Saga. Optimized performance
              and integrated Storybook for improved developer experience.
            </p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">React</span>
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">Redux
                Saga</span>
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">Storybook</span>
            </div>
            <div class="text-xs text-gray-500 dark:text-gray-400">
              <strong>Team:</strong> 6 Frontend, 8 Backend, 2 DevOps, 1 PO, 1 PM, 2 BI
            </div>
          </div>

          <!-- Ecommerce Platform -->
          <div class="card dark:bg-dark-900 p-6 animate-slide-up" style="animation-delay: 0.2s;">
            <h3 class="text-xl font-bold mb-2">Ecommerce Platform</h3>
            <p class="text-primary-600 dark:text-primary-400 text-sm mb-3">Alfaprint • April 2021 - September 2021</p>
            <p class="text-gray-600 dark:text-gray-400 mb-4">
              Developed a printer sales platform with React and Bootstrap, achieving 99% page speed optimization
              and significant SEO improvements.
            </p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">React</span>
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">Bootstrap</span>
              <span
                class="px-2 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded text-xs">SEO</span>
            </div>
            <div class="text-xs text-gray-500 dark:text-gray-400">
              <strong>Achievement:</strong> 99% PageSpeed Score
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
