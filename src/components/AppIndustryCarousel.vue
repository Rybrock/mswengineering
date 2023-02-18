<template>
    <div class="my-10 md:my-28 bg-red-500 p-4">
        <div>
            <h3 class="font-bold text-2xl text-white mb-10">Industries we cover</h3>
        </div>
        <div class="w-full">
            <swiper class="swiper" :modules="modules" :slides-per-view="3" :space-between="5" @swiper="onSwiper"
                @slideChange="onSlideChange" :autoplay="true" 
                :breakpoints="{
                    '340': {
                        slidesPerView: 1,
                        spaceBetween: 40
                    },
                    '768': {
                        slidesPerView: 3,
                        spaceBetween: 40
                    },
                    '1024': {
                        slidesPerView: 3,
                        spaceBetween: 50
                    }
                }" navigation>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food.jpg" alt="">
                        <p class="absolute bottom-5 lg:bottom-10 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/beverages.jpg" alt="">
                        <p class="absolute bottom-5 lg:bottom-10 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">Beverages</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/pharma.jpg" alt="">
                        <p class="absolute bottom-5 lg:bottom-10 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">Pharmaceutical</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/chem.jpg" alt="" height="280">
                        <p class="absolute bottom-5 lg:bottom-10 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">Chemical</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/paper.jpg" alt="">
                        <p class="absolute bottom-5 lg:bottom-10 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">Paper & pulp</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/oem.jpg" alt="">
                        <p class="absolute bottom-5 lg:bottom-10 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">OEM's</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/ecomm.jpeg" alt="">
                        <p class="absolute bottom-5 lg:bottom-10 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">E-commerce distribution</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/fmcg.jpg" alt="">
                        <p class="absolute bottom-5 lg:bottom-20 left-10 bg-slate-300 opacity-100 font-bold text-black px-4 py-2 rounded-xl">General FMCG</p>
                    </div>
                </swiper-slide>
            </swiper>
        </div>

    </div>
</template>
<script>
// Import Swiper Vue.js components
import { Autoplay, Navigation } from 'swiper'
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        const onSwiper = (swiper) => {
            console.log(swiper);
        };
        const onSlideChange = () => {
            console.log('slide change');
        };
        return {
            onSwiper,
            onSlideChange,
            modules: [Autoplay, Navigation]
        };
    },
};
</script>

<style scoped>
img {
    width: 100%;
    /* max-width: 450px; */
    height: 100%;
    /* max-height: 260px !important; */
}

.swiper {
    width: 100%;
    height: 100%;
    max-height: 300px !important;
    padding-bottom: 2%;
}
@media only screen and (max-width: 340px) {
    img {
    width: 100%;
    height: 100%;
    max-height: 240px !important;
    padding-bottom: 20% !important;
}
}
</style>