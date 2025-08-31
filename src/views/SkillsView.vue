<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section
      class="section-padding bg-gradient-to-br from-primary-50 via-white to-purple-50 dark:from-dark-900 dark:via-dark-800 dark:to-dark-900">
      <div class="container-custom">
        <div class="max-w-4xl mx-auto text-center">
          <h1 class="text-5xl md:text-6xl font-bold mb-6 animate-slide-up">
            {{ $t('skills.title') }}
          </h1>
          <p class="text-xl text-gray-600 dark:text-gray-400 mb-8 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('skills.subtitle') }}
          </p>
        </div>
      </div>
    </section>

    <!-- Frontend Skills -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('skills.frontend') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('skills.frontendDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div v-for="(skill, index) in frontendSkills" :key="skill.name"
            class="card dark:bg-dark-900 p-6 text-center animate-slide-up"
            :style="{ animationDelay: `${0.1 * index}s` }">
            <div
              class="w-16 h-16 mx-auto mb-4 bg-primary-100 dark:bg-primary-900 rounded-lg flex items-center justify-center">
              <component :is="skill.icon" class="w-8 h-8 text-primary-600" />
            </div>
            <h3 class="font-semibold text-lg mb-2">{{ skill.name }}</h3>
            <p class="text-gray-600 dark:text-gray-400 text-sm mb-4">{{ skill.description }}</p>

          </div>
        </div>
      </div>
    </section>

    <!-- State Management -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('skills.stateManagement') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('skills.stateManagementDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div v-for="(skill, index) in stateManagementSkills" :key="skill.name"
            class="card  p-6 text-center animate-slide-up" :style="{ animationDelay: `${0.1 * index}s` }">
            <div
              class="w-16 h-16 mx-auto mb-4 bg-purple-100 dark:bg-purple-900 rounded-lg flex items-center justify-center">
              <component :is="skill.icon" class="w-8 h-8 text-purple-600" />
            </div>
            <h3 class="font-semibold text-lg mb-2">{{ skill.name }}</h3>
            <p class="text-gray-600 dark:text-gray-400 text-sm mb-4">{{ skill.description }}</p>

          </div>
        </div>
      </div>
    </section>

    <!-- Backend & Tools -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('skills.backend') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('skills.backendDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div v-for="(skill, index) in backendSkills" :key="skill.name"
            class="card dark:bg-dark-900 p-6 text-center animate-slide-up"
            :style="{ animationDelay: `${0.1 * index}s` }">
            <div
              class="w-16 h-16 mx-auto mb-4 bg-green-100 dark:bg-green-900 rounded-lg flex items-center justify-center">
              <component :is="skill.icon" class="w-8 h-8 text-green-600" />
            </div>
            <h3 class="font-semibold text-lg mb-2">{{ skill.name }}</h3>
            <p class="text-gray-600 dark:text-gray-400 text-sm mb-4">{{ skill.description }}</p>

          </div>
        </div>
      </div>
    </section>

    <!-- Testing & Quality -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('skills.testing') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('skills.testingDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div v-for="(skill, index) in testingSkills" :key="skill.name" class="card  p-6 text-center animate-slide-up"
            :style="{ animationDelay: `${0.1 * index}s` }">
            <div
              class="w-16 h-16 mx-auto mb-4 bg-orange-100 dark:bg-orange-900 rounded-lg flex items-center justify-center">
              <component :is="skill.icon" class="w-8 h-8 text-orange-600" />
            </div>
            <h3 class="font-semibold text-lg mb-2">{{ skill.name }}</h3>
            <p class="text-gray-600 dark:text-gray-400 text-sm mb-4">{{ skill.description }}</p>

          </div>
        </div>
      </div>
    </section>

    <!-- Additional Skills -->
    <section class="section-padding bg-white dark:bg-dark-800">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('skills.additionalSkills') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('skills.additionalSkillsDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div v-for="(category, index) in additionalSkills" :key="category.name"
            class="card dark:bg-dark-900 p-6 animate-slide-up" :style="{ animationDelay: `${0.1 * index}s` }">
            <h3 class="text-xl font-bold mb-4">{{ category.name }}</h3>
            <div class="flex flex-wrap gap-2">
              <span v-for="skill in category.skills" :key="skill"
                class="px-3 py-1 bg-primary-100 dark:bg-primary-900 text-primary-700 dark:text-primary-300 rounded-full text-sm font-medium">
                {{ skill }}
              </span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Skills Summary -->
    <section class="section-padding bg-gray-50 dark:bg-dark-900">
      <div class="container-custom">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold mb-4 animate-slide-up">{{ $t('skills.skillsSummary') }}</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 animate-slide-up" style="animation-delay: 0.2s;">
            {{ $t('skills.skillsSummaryDesc') }}
          </p>
        </div>

        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div class="card  p-6 text-center animate-slide-up">
            <div class="text-4xl font-bold gradient-text mb-2">5+</div>
            <p class="text-gray-600 dark:text-gray-400">Years Experience</p>
          </div>

          <div class="card  p-6 text-center animate-slide-up" style="animation-delay: 0.1s;">
            <div class="text-4xl font-bold gradient-text mb-2">15+</div>
            <p class="text-gray-600 dark:text-gray-400">Technologies</p>
          </div>

          <div class="card  p-6 text-center animate-slide-up" style="animation-delay: 0.2s;">
            <div class="text-4xl font-bold gradient-text mb-2">3</div>
            <p class="text-gray-600 dark:text-gray-400">Major Frameworks</p>
          </div>

          <div class="card  p-6 text-center animate-slide-up" style="animation-delay: 0.3s;">
            <div class="text-4xl font-bold gradient-text mb-2">100%</div>
            <p class="text-gray-600 dark:text-gray-400">Responsive Design</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
import {
  CodeBracketIcon,
  GlobeAltIcon,
  CommandLineIcon,
  CpuChipIcon,
  ServerIcon,
  WrenchScrewdriverIcon,
  BeakerIcon,
  DocumentTextIcon,
  CogIcon,
  ShieldCheckIcon
} from '@heroicons/vue/24/outline'

const frontendSkills = [
  {
    name: 'React',
    description: 'Building interactive UIs with modern React patterns',
    icon: CodeBracketIcon,
    proficiency: 95
  },
  {
    name: 'Vue.js',
    description: 'Creating reactive and scalable applications',
    icon: GlobeAltIcon,
    proficiency: 90
  },
  {
    name: 'Angular',
    description: 'Enterprise-level application development',
    icon: CommandLineIcon,
    proficiency: 85
  },
  {
    name: 'TypeScript',
    description: 'Type-safe development for better code quality',
    icon: CpuChipIcon,
    proficiency: 92
  }
]

const stateManagementSkills = [
  {
    name: 'Redux',
    description: 'Predictable state management for React apps',
    icon: CogIcon,
    proficiency: 90
  },
  {
    name: 'React Query',
    description: 'Server state management and caching',
    icon: WrenchScrewdriverIcon,
    proficiency: 88
  },
  {
    name: 'Redux Saga',
    description: 'Side effect management for Redux',
    icon: WrenchScrewdriverIcon,
    proficiency: 85
  },
  {
    name: 'Context API',
    description: 'React\'s built-in state management',
    icon: DocumentTextIcon,
    proficiency: 92
  }
]

const backendSkills = [
  {
    name: 'Node.js',
    description: 'Server-side JavaScript runtime',
    icon: ServerIcon,
    proficiency: 80
  },
  {
    name: 'NestJS',
    description: 'Progressive Node.js framework',
    icon: CpuChipIcon,
    proficiency: 75
  },
  {
    name: 'Express.js',
    description: 'Fast, unopinionated web framework',
    icon: CommandLineIcon,
    proficiency: 82
  },
  {
    name: 'Git',
    description: 'Version control and collaboration',
    icon: CodeBracketIcon,
    proficiency: 90
  }
]

const testingSkills = [
  {
    name: 'Jest',
    description: 'JavaScript testing framework',
    icon: BeakerIcon,
    proficiency: 85
  },
  {
    name: 'Cypress',
    description: 'End-to-end testing framework',
    icon: ShieldCheckIcon,
    proficiency: 80
  },
  {
    name: 'Storybook',
    description: 'UI component development environment',
    icon: DocumentTextIcon,
    proficiency: 88
  },
  {
    name: 'Testing',
    description: 'Unit and integration testing',
    icon: BeakerIcon,
    proficiency: 85
  }
]

const additionalSkills = [
  {
    name: 'Styling & UI',
    skills: ['Tailwind CSS', 'Chakra UI', 'SCSS', 'Bootstrap', 'CSS3', 'HTML5']
  },
  {
    name: 'Development Tools',
    skills: ['Docker', 'Webpack', 'Vite', 'ESLint', 'Prettier', 'Storybook']
  },
  {
    name: 'APIs & Data',
    skills: ['RESTful APIs', 'GraphQL', 'MongoDB', 'MySQL', 'JSON', 'XML']
  }
]
</script>
