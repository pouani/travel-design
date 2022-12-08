<template lang="">
    <div>
        <div class="px-4 md:pl-24 md:px-0">
            <Header />
            <About />
            <Feature />
            <Slide />
        </div>
        <Footer />
    </div>
</template>
<script setup>
import Header from '@/components/Header.vue';
import About from '@/components/About.vue';
import Footer from '@/components/Footer.vue';
import Slide from '@/components/Slide.vue';
import Feature from '@/components/Feature.vue';
</script>
<style lang="">
    
</style>