<template>
    <div class="footer-links flex flex-wrap justify-between items-center w-[462px]">
        <div class="product">
            <p class="title uppercase font-bold text-[16px]" >Products</p>
            <ul class="flex flex-col gap-[20px] mt-[20px]">
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Living Room</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Dining & Kitchen</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">BedRoom</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Outdoor</router-link>
                </li>
            </ul>
        </div>
        
        <div class="about">
            <p class="title uppercase font-bold text-[16px]" >About us</p>
            <ul class="flex flex-col gap-[20px] mt-[20px]">
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Our Team</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Services</router-link>
                </li>
               
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Shop Page</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">FAQs</router-link>
                </li>
            </ul>
        </div>
        <div class="follow">
            <p class="title uppercase font-bold text-[16px]" >Follow us</p>
            <ul class="flex flex-col gap-[20px] mt-[20px]">
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Facebook</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Instagram</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Twitter</router-link>
                </li>
                <li>
                    <router-link to="/home" class="hover:text-[#EFF422] duration-200 text-[16px]">Behance</router-link>
                </li>
            </ul>
        </div>
        
    </div>
</template>