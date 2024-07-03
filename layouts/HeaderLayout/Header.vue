<script setup lang="ts">
import HeaderLinks from './components/HeaderLinks.vue'
import HeaderCart from './components/HeaderCart.vue'
import HeaderMainLogo from './components/HeaderMainLogo.vue'
</script>
<template>
    <header class="header py-[20px] ">
        <div class="container flex items-center justify-between">
<HeaderMainLogo/>
                <HeaderLinks />
                <HeaderCart />
             
        </div>
    </header>
</template>