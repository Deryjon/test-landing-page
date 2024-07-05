<script lang="ts" setup>
import card1 from '../../assets/img/card-1.jpg';
import card2 from '../../assets/img/card-2.jpg';
import card3 from '../../assets/img/card-3.jpg';

const cardData = [
    {
        text: 'Our Philosophy',
        img: card1,
    },
    {
        text: 'Starting Projects',
        img: card2,
    },
    {
        text: 'Function And Beauty',
        img: card3,
    },
];
</script>

<template>
    <section class="service pt-[310px] py-[150px]">
        <div class="container">

            <h2 class="text-[50px] font-bold uppercase text-white">our services</h2>

            <div class="cards flex justify-between mt-[68px] ">
                <div class="card w-[410px] h-[307px] relative " v-for="card in cardData">
                    <img :src="card.img" alt="" class="w-full h-full rounded-[15px]">
                    <p class="text-white absolute top-[254px] left-[30px] font-bold text-[24px]">{{ card.text }}</p>
                    <img src="../../assets/icons/icon-arrow.svg" alt="" class="absolute bottom-[0px] right-[0px] rounded-br-[15px]">
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
.service {
    background-image: url("../../assets/img/Bg.jpg");
    background-size: cover;
}
</style>