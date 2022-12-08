<template lang="html">
    <div class='content drop-shadow-2xl pb-4'>
      <div class="content-btn flex bg-white md:max-w-fit">
        <button class="px-12 py-3">Buy</button>
        <button class="bg-gray-200 px-12 py-3">Sell</button>
        <button class="bg-gray-200 px-12 py-3">Rent</button>
        </div>
      <div>
        <ul class="wrapper px-4 py-3 flex gap-8">
            <li class="border-r pr-12">
                <p class="flex items-center gap-2">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z" />
                        <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1115 0z" />
                    </svg>
                    <span>Location</span>
                </p>
                <h4 class="px-1 py-3">Semarang, Indenosia</h4>
            </li>
            <li class="pr-12">
                <p class="flex items-center gap-2">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
                    </svg>
                    <span>Style</span>
                </p>
                <h4 class="px-1 py-3">Modern, Minimalist</h4>
            </li>
        </ul>
      </div>
    </div>
  </template>
  
  <script>
  import Tab from './Tab.vue'
  import Tabs from './Tabs.vue'
  
  export default {
    components: {
      Tab,
      Tabs
    },
    data () {
      return {
        mode: 'dark'
      }
    },
    methods: {
      changeStyle () {
        if (this.mode === 'dark') {
          this.mode = 'light'
        } else {
          this.mode = 'dark'
        }
      }
    }
  }
  </script>
