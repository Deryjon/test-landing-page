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

                <div class="wrapper flex flex-wrap justify-between mt-[60px]">
                    <div class="card w-[410px] h-[410px] relative " v-for="card in news">
                        <img :src='card.photo' alt="" class="rounded-[15px]">
                        <div class="texts absolute bottom-[10px] left-[10px] w-[390px] flex items-center justify-between  bg-[#FFFFFF66] px-[15px] py-[20px]">
                            <div class="date-name w-[250px] text-white">
                                <p>{{ card.data }}</p>
                                <p class="text-[18px] font-extrabold">{{ card.name }}</p>
                            </div>
                            <div class="arrow text-white">
<img src="../../assets/icons/white-arrow.svg" alt="">
                            </div>
                        </div>
                    </div>
                </div>
        </div>
    </section>
</template>