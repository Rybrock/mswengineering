<template>
    <div class="mt-24 bg-red-500 p-4">
        <div>
            <h3 class="font-bold text-2xl text-white">Industries we cover</h3>
        </div>
        <div class="flex flex-col">
            <swiper class="swiper" :slides-per-view="3" :space-between="5" @swiper="onSwiper"
                @slideChange="onSlideChange" :autoplay="true" :breakpoints="{
                    '340': {
        slidesPerView: 1,
    },
    '640': {
        slidesPerView: 1,
    },
    '768': {
        slidesPerView: 1,
        spaceBetween: 40
    },
}">
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="relative">
                        <img src="../assets/food-processing-and-packaging---industry-overview.webp" width="600"
                            height="246px" alt="">
                        <p class="absolute bottom-5 left-10 bg-black text-white px-4 py-2 rounded-xl">Food</p>
                    </div>
                </swiper-slide>
            </swiper>
        </div>

    </div>
</template>
<script>
// Import Swiper Vue.js components
import { Autoplay } from 'swiper'
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
            modules: [Autoplay]
        };
    },
};
</script>

<style scoped>
.swiper-slide img {
    width: 100%;
    max-width: 450px;
    height: 100%;
    max-height: 240px !important;
}

.swiper {
    width: 100%;
    height: 50%;
    padding: 20px;
}
</style>