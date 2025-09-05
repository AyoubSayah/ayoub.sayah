<template>

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
                                <svg class="w-6 h-6 text-primary-600" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                </svg>
                            </div>
                            <div>
                                <h3 class="text-lg font-bold mb-2">Angular Developer Certification</h3>
                                <p class="text-primary-600 dark:text-primary-400 text-sm mb-2">Certficates.dev</p>
                                <p class="text-gray-600 dark:text-gray-400 text-sm">Advanced Angular concepts and best
                                    practices</p>
                            </div>
                        </div>
                    </div>

                    <div class="card p-6 animate-slide-up" style="animation-delay: 0.1s;">
                        <div class="flex items-start">
                            <div
                                class="w-12 h-12 bg-green-100 dark:bg-green-900 rounded-lg flex items-center justify-center mr-4 flex-shrink-0">
                                <svg class="w-6 h-6 text-green-600" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                </svg>
                            </div>
                            <div>
                                <h3 class="text-lg font-bold mb-2">Vue.js Developer Certification</h3>
                                <p class="text-green-600 dark:text-green-400 text-sm mb-2">Certficates.dev</p>
                                <p class="text-gray-600 dark:text-gray-400 text-sm">Vue 3 Composition API and ecosystem
                                </p>
                            </div>
                        </div>
                    </div>

                    <div class="card p-6 animate-slide-up" style="animation-delay: 0.2s;">
                        <div class="flex items-start">
                            <div
                                class="w-12 h-12 bg-purple-100 dark:bg-purple-900 rounded-lg flex items-center justify-center mr-4 flex-shrink-0">
                                <svg class="w-6 h-6 text-purple-600" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
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
                                <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
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
</template>