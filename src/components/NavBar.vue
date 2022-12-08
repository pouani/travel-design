<template lang="">
    <nav x-data="{ isOpen: false }" class="relative bg-white">
    <div class="container md:pr-2 py-3 mx-auto md:flex">
        <div class="flex items-center justify-between">
            <div class="logo flex items-center gap-1">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-8 h-8">
                    <path d="M6 3a3 3 0 00-3 3v2.25a3 3 0 003 3h2.25a3 3 0 003-3V6a3 3 0 00-3-3H6zM15.75 3a3 3 0 00-3 3v2.25a3 3 0 003 3H18a3 3 0 003-3V6a3 3 0 00-3-3h-2.25zM6 12.75a3 3 0 00-3 3V18a3 3 0 003 3h2.25a3 3 0 003-3v-2.25a3 3 0 00-3-3H6zM17.625 13.5a.75.75 0 00-1.5 0v2.625H13.5a.75.75 0 000 1.5h2.625v2.625a.75.75 0 001.5 0v-2.625h2.625a.75.75 0 000-1.5h-2.625V13.5z" />
                </svg>

                <a class="text-2xl font-bold text-gray-800 transition-colors duration-300 transform lg:text-3xl hover:text-gray-700" href="#">
                    GUBUKUH
                </a>
            </div>

            <!-- Mobile menu button -->
            <div class="flex lg:hidden">
                <button @click="isOpen = !isOpen" type="button" class="text-gray-500 hover:text-gray-600 focus:outline-none focus:text-gray-600 " aria-label="toggle menu">
                    <svg v-if="!isOpen" xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M4 8h16M4 16h16" />
                    </svg>
            
                    <svg v-if="isOpen" xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                    </svg>
                </button>
            </div>
        </div>

        <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
        <div x-cloak :class="[isOpen ? 'translate-x-0 opacity-100 ' : 'opacity-0 -translate-x-full']" class="nav-link absolute inset-x-0 z-20 w-full px-6 py-4 transition-all duration-300 ease-in-out bg-white md:mt-0 md:p-0 md:top-0 
        md:relative md:opacity-100 md:translate-x-0 md:flex md:items-center md:justify-between">
            <div class="flex flex-col px-2 -mx-4 md:flex-row md:mx-10 md:py-0">
                <a href="#" class="active px-2.5 py-2 text-gray-700 transition-colors duration-300 transform rounded-lg hover:bg-gray-100 md:mx-2">Home</a>
                <a href="#" class="px-2.5 py-2 text-gray-700 transition-colors duration-300 transform rounded-lg hover:bg-gray-100 md:mx-2">Products</a>
                <a href="#" class="px-2.5 py-2 text-gray-700 transition-colors duration-300 transform rounded-lg hover:bg-gray-100 md:mx-2">About Us</a>
                <a href="#" class="px-2.5 py-2 text-gray-700 transition-colors duration-300 transform rounded-lg hover:bg-gray-100 md:mx-2">Support</a>
            </div>

            <div class="relative mt-4 md:mt-0">
                <button class="btn">Log in</button>
            </div>
        </div>
    </div>
</nav>
</template>
<script setup>
import { ref } from 'vue'

const isOpen = ref(false)
</script>