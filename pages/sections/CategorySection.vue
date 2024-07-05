<script lang="ts" setup>
import { ref } from 'vue'

const categoryData = [
    {
        text: 'Decorate',
    },
    {
        text: 'Furniture',
    },
    {
        text: 'Living Room',
    },
    {
        text: 'Dining & Kitchen',
    },
    {
        text: 'Bedroom',
    },
    {
        text: 'Our Door',
    },
    {
        text: 'Home Office',
    },
    {
        text: 'Rugs',
    },
    {
        text: 'Lighting',
    },
    {
        text: 'Storage & Modular',
    },
]

const activeButton = ref<number | null>(1) // дефолт - Furniture
function handleClick(index: number) {
    activeButton.value = activeButton.value === index ? null : index
}
</script>
<template>
    <section class="category py-[100px]">
        <div class="container flex flex-wrap gap-[30px] justify-center">
            <button
                class="rounded-[34px] border-2 py-[20px] px-[70px] "
                :class="{ 'bg-[#EFF422]': activeButton === index }"
                v-for="(data, index) in categoryData"
                :key="index"
                @click="handleClick(index)"
            >
                {{ data.text }}
            </button>
        </div>
    </section>
</template>
