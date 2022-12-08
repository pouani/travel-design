<template lang="">
    <div class="grid grid-cols-1 md:grid-cols-2 md:pr-24">
        <div>
            <img src="@/assets/feature-item-1.png" alt="">
        </div>
        <div>
            <h2>Features Our Provide</h2>
            <p>We always strive to provide premium services at 
                affordable prices for customer satisfaction.</p>
            <ul class="mt-6">
                <li v-for="item in 4" :key="index"
                class="bg-white drop-shadow-2xl px-3 py-5 rounded-md flex gap-6 mt-6">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v12m-3-2.818l.879.659c1.171.879 3.07.879 4.242 0 1.172-.879 1.172-2.303 0-3.182C13.536 12.219 12.768 12 12 12c-.725 0-1.45-.22-2.003-.659-1.106-.879-1.106-2.303 0-3.182s2.9-.879 4.006 0l.415.33M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                    <p>Affordable Prices</p>
                </li>
            </ul>
            <div class="mt-5">
                <button class="bg-blue-400 py-4 px-8 text-white">
                    More information ->
                </button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="">
    
</style>