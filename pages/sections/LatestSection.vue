<script lang="ts" setup>
import Title from '../../components/Title.vue'
import photo1 from '../../assets/img/news-1.jpg'
import photo2 from '../../assets/img/news-2.jpg'
import photo3 from '../../assets/img/news-3.jpg'
const news = [
    {
        data: 'August 1, 2023',
        name: 'Ipsum suspendisse ultrices',
        photo: photo1,
    },
    {
        data: 'August 1, 2023',
        name: 'Ut tortor pretium viverra',
        photo: photo2,
    },
    {
        data: 'August 1, 2023',
        name: 'Dignissim cras tincidunt',
        photo: photo3,
    },
]
</script>
<template>
    <section class="latest bg-[#FAFAF4] py-[100px]">
        <div class="container">
            <Title class="">latest news</Title>
            <p class="text-center w-[500px] mx-auto text-[16px] mt-[20px]">Lorem ipsum dolor sit amet, consectetur
                adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>

                <div class="wrapper flex flex-wrap justify-between mt-[60p]">
                    <div class="card w-[410px] h-[410px]" v-for="card in news">
                        <img :src='card.photo' alt="">
                    </div>
                </div>
        </div>
    </section>
</template>