<script setup lang="ts">
import HeaderLinks from './components/HeaderLinks.vue'
import HeaderPhone from './components/HeaderPhone.vue'
import HeaderLogin from './components/HeaderLogin.vue'
import HeaderMainLogo from './components/HeaderMainLogo.vue'
</script>
<template>
    <header class="header py-[10px] bg-[#F6F7FB]">
        <div class="container ">
            <div class="header-small  flex justify-between ">

                <HeaderLinks />
                <div class=" flex gap-[60px]">

                    <HeaderPhone />
                    <HeaderLogin />
                </div>
            </div>
        </div>
    </header>
    <div class="header-main py-[4]">
        <div class="container">

            <HeaderMainLogo/>
        </div>
    </div>
</template>