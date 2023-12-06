<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
</script>

<template>
    <Head title="Dashboard" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 dark:text-gray-200 leading-tight">Dashboard</h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <div class="bg-white dark:bg-gray-800 overflow-hidden shadow-sm sm:rounded-lg">
                    <div class="p-6 text-gray-900 dark:text-gray-100">You're logged in!</div>
                    <div class="p-4">
                        <button type="button"
                            class="py-3 px-4 inline-flex items-center gap-x-2 text-sm font-semibold rounded-lg border border-transparent bg-blue-600 text-white hover:bg-blue-700 disabled:opacity-50 disabled:pointer-events-none dark:focus:outline-none dark:focus:ring-1 dark:focus:ring-gray-600">
                            Solid
                        </button>
                        <button type="button"
                            class="py-3 px-4 inline-flex items-center gap-x-2 text-sm font-semibold rounded-lg border border-gray-200 text-gray-500 hover:border-blue-600 hover:text-blue-600 disabled:opacity-50 disabled:pointer-events-none dark:border-gray-700 dark:text-gray-400 dark:hover:text-blue-500 dark:hover:border-blue-600 dark:focus:outline-none dark:focus:ring-1 dark:focus:ring-gray-600">
                            Outline
                        </button>
                        <button type="button"
                            class="px-4 inline-flex items-center gap-x-2 text-sm font-semibold rounded-lg border border-transparent text-blue-600 hover:bg-blue-100 hover:text-blue-800 disabled:opacity-50 disabled:pointer-events-none dark:text-blue-500 dark:hover:bg-blue-800/30 dark:hover:text-blue-400 dark:focus:outline-none dark:focus:ring-1 dark:focus:ring-gray-600">
                            Ghost
                        </button>
                        <button type="button"
                            class="py-3 px-4 inline-flex items-center gap-x-2 text-sm font-semibold rounded-lg border border-transparent bg-blue-100 text-blue-800 hover:bg-blue-200 disabled:opacity-50 disabled:pointer-events-none dark:hover:bg-blue-900 dark:text-blue-400 dark:focus:outline-none dark:focus:ring-1 dark:focus:ring-gray-600">
                            Soft
                        </button>
                        <button type="button"
                            class="py-3 px-4 inline-flex items-center gap-x-2 text-sm font-medium rounded-lg border border-gray-200 bg-white text-gray-800 shadow-sm hover:bg-gray-50 disabled:opacity-50 disabled:pointer-events-none dark:bg-slate-900 dark:border-gray-700 dark:text-white dark:hover:bg-gray-800 dark:focus:outline-none dark:focus:ring-1 dark:focus:ring-gray-600">
                            White
                        </button>
                        <button type="button"
                            class="py-3 px-4 inline-flex items-center gap-x-2 text-sm font-semibold rounded-lg border border-transparent text-blue-600 hover:text-blue-800 disabled:opacity-50 disabled:pointer-events-none dark:text-blue-500 dark:hover:text-blue-400 dark:focus:outline-none dark:focus:ring-1 dark:focus:ring-gray-600">
                            Link
                        </button>
                    </div>
                    <div class="p-4">
                        <div class="hs-accordion-group">
                            <div class="hs-accordion active bg-white border -mt-px first:rounded-t-lg last:rounded-b-lg dark:bg-gray-800 dark:border-gray-700"
                                id="hs-bordered-heading-one">
                                <button
                                    class="hs-accordion-toggle hs-accordion-active:text-blue-600 inline-flex items-center gap-x-3 w-full font-semibold text-start text-gray-800 py-4 px-5 hover:text-gray-500 disabled:opacity-50 disabled:pointer-events-none dark:hs-accordion-active:text-blue-500 dark:text-gray-200 dark:hover:text-gray-400 dark:focus:outline-none dark:focus:text-gray-400"
                                    aria-controls="hs-basic-bordered-collapse-one">
                                    <svg class="hs-accordion-active:hidden block w-4 h-4" xmlns="http://www.w3.org/2000/svg"
                                        width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                                        stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14" />
                                        <path d="M12 5v14" />
                                    </svg>
                                    <svg class="hs-accordion-active:block hidden w-4 h-4" xmlns="http://www.w3.org/2000/svg"
                                        width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                                        stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14" />
                                    </svg>
                                    Accordion #1
                                </button>
                                <div id="hs-basic-bordered-collapse-one"
                                    class="hs-accordion-content w-full overflow-hidden transition-[height] duration-300"
                                    aria-labelledby="hs-bordered-heading-one">
                                    <div class="pb-4 px-5">
                                        <p class="text-gray-800 dark:text-gray-200">
                                            <em>This is the third item's accordion body.</em> It is hidden by default, until
                                            the collapse plugin adds the appropriate classes that we use to style each
                                            element. These classes control the overall appearance, as well as the showing
                                            and hiding via CSS transitions.
                                        </p>
                                    </div>
                                </div>
                            </div>

                            <div class="hs-accordion bg-white border -mt-px first:rounded-t-lg last:rounded-b-lg dark:bg-gray-800 dark:border-gray-700"
                                id="hs-bordered-heading-two">
                                <button
                                    class="hs-accordion-toggle hs-accordion-active:text-blue-600 inline-flex items-center gap-x-3 w-full font-semibold text-start text-gray-800 py-4 px-5 hover:text-gray-500 disabled:opacity-50 disabled:pointer-events-none dark:hs-accordion-active:text-blue-500 dark:text-gray-200 dark:hover:text-gray-400 dark:focus:outline-none dark:focus:text-gray-400"
                                    aria-controls="hs-basic-bordered-collapse-two">
                                    <svg class="hs-accordion-active:hidden block w-4 h-4" xmlns="http://www.w3.org/2000/svg"
                                        width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                                        stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14" />
                                        <path d="M12 5v14" />
                                    </svg>
                                    <svg class="hs-accordion-active:block hidden w-4 h-4" xmlns="http://www.w3.org/2000/svg"
                                        width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                                        stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14" />
                                    </svg>
                                    Accordion #2
                                </button>
                                <div id="hs-basic-bordered-collapse-two"
                                    class="hs-accordion-content hidden w-full overflow-hidden transition-[height] duration-300"
                                    aria-labelledby="hs-bordered-heading-two">
                                    <div class="pb-4 px-5">
                                        <p class="text-gray-800 dark:text-gray-200">
                                            <em>This is the second item's accordion body.</em> It is hidden by default,
                                            until the collapse plugin adds the appropriate classes that we use to style each
                                            element. These classes control the overall appearance, as well as the showing
                                            and hiding via CSS transitions.
                                        </p>
                                    </div>
                                </div>
                            </div>

                            <div class="hs-accordion bg-white border -mt-px first:rounded-t-lg last:rounded-b-lg dark:bg-gray-800 dark:border-gray-700"
                                id="hs-bordered-heading-three">
                                <button
                                    class="hs-accordion-toggle hs-accordion-active:text-blue-600 inline-flex items-center gap-x-3 w-full font-semibold text-start text-gray-800 py-4 px-5 hover:text-gray-500 disabled:opacity-50 disabled:pointer-events-none dark:hs-accordion-active:text-blue-500 dark:text-gray-200 dark:hover:text-gray-400 dark:focus:outline-none dark:focus:text-gray-400"
                                    aria-controls="hs-basic-bordered-collapse-three">
                                    <svg class="hs-accordion-active:hidden block w-4 h-4" xmlns="http://www.w3.org/2000/svg"
                                        width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                                        stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14" />
                                        <path d="M12 5v14" />
                                    </svg>
                                    <svg class="hs-accordion-active:block hidden w-4 h-4" xmlns="http://www.w3.org/2000/svg"
                                        width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                                        stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14" />
                                    </svg>
                                    Accordion #3
                                </button>
                                <div id="hs-basic-bordered-collapse-three"
                                    class="hs-accordion-content hidden w-full overflow-hidden transition-[height] duration-300"
                                    aria-labelledby="hs-bordered-heading-three">
                                    <div class="pb-4 px-5">
                                        <p class="text-gray-800 dark:text-gray-200">
                                            <em>This is the first item's accordion body.</em> It is hidden by default, until
                                            the collapse plugin adds the appropriate classes that we use to style each
                                            element. These classes control the overall appearance, as well as the showing
                                            and hiding via CSS transitions.
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="p-4">
                            <!-- Slider -->
                            <div data-hs-carousel='{
            "loadingClasses": "opacity-0"
          }' class="relative">
                                <div class="hs-carousel relative overflow-hidden w-full min-h-[350px] bg-white rounded-lg">
                                    <div
                                        class="hs-carousel-body absolute top-0 bottom-0 start-0 flex flex-nowrap transition-transform duration-700 opacity-0">
                                        <div class="hs-carousel-slide">
                                            <div class="flex justify-center h-full bg-gray-100 p-6">
                                                <span class="self-center text-4xl transition duration-700">First
                                                    slide</span>
                                            </div>
                                        </div>
                                        <div class="hs-carousel-slide">
                                            <div class="flex justify-center h-full bg-gray-200 p-6">
                                                <span class="self-center text-4xl transition duration-700">Second
                                                    slide</span>
                                            </div>
                                        </div>
                                        <div class="hs-carousel-slide">
                                            <div class="flex justify-center h-full bg-gray-300 p-6">
                                                <span class="self-center text-4xl transition duration-700">Third
                                                    slide</span>
                                            </div>
                                        </div>
                                    </div>
                                </div>

                                <button type="button"
                                    class="hs-carousel-prev hs-carousel:disabled:opacity-50 disabled:pointer-events-none absolute inset-y-0 start-0 inline-flex justify-center items-center w-[46px] h-full text-gray-800 hover:bg-gray-800/[.1]">
                                    <span class="text-2xl" aria-hidden="true">
                                        <svg class="w-4 h-4" xmlns="http://www.w3.org/2000/svg" width="16" height="16"
                                            fill="currentColor" viewBox="0 0 16 16">
                                            <path fill-rule="evenodd"
                                                d="M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z" />
                                        </svg>
                                    </span>
                                    <span class="sr-only">Previous</span>
                                </button>
                                <button type="button"
                                    class="hs-carousel-next hs-carousel:disabled:opacity-50 disabled:pointer-events-none absolute inset-y-0 end-0 inline-flex justify-center items-center w-[46px] h-full text-gray-800 hover:bg-gray-800/[.1]">
                                    <span class="sr-only">Next</span>
                                    <span class="text-2xl" aria-hidden="true">
                                        <svg class="w-4 h-4" xmlns="http://www.w3.org/2000/svg" width="16" height="16"
                                            fill="currentColor" viewBox="0 0 16 16">
                                            <path fill-rule="evenodd"
                                                d="M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z" />
                                        </svg>
                                    </span>
                                </button>
                        </div>
                        <!-- End Slider -->
                    </div>
                </div>
            </div>
        </div>
    </div>
</AuthenticatedLayout></template>
