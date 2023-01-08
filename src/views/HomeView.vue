<template>
  <div class="home">
    <div class="mb-4">
      <app-image-block/>
    </div>
    <app-about-block/>
    <app-industry-carousel/>
    <!-- <app-testimonial-carousel/> -->
  </div>
</template>

<script>
// @ is an alias to /src
import AppImageBlock from '@/components/AppImageBlock.vue';
import AppAboutBlock from '@/components/AppAboutBlock.vue';
import AppIndustryCarousel from '@/components/AppIndustryCarousel.vue';
// import AppTestimonialCarousel from '@/components/AppTestimonialCarousel.vue';
export default {
  name: 'HomeView',
  components: {
    AppImageBlock,
    AppAboutBlock,
    AppIndustryCarousel,
    // AppTestimonialCarousel
  }
}
</script>