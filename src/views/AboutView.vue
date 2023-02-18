<template>
  <div class="about w-full p-2">
    <div class="p-2">
      <!-- <h1 class="fs-3 fw-bold text-start p-2 text-muted">Overview of MSW and the areas we cover</h1> -->
    </div>
    <div class="mx-auto w-full flex flex-col md:flex-row md:my-16">
      <div class="about-info text-center mx-2 w-full">
        <h3 class="text-red-700 text-start p-2 text-lg">Our Story</h3>
        <p class="p-2 text-start">
          A recruitment company that was founded on the basic principle of
          ensuring that the client and candidate are our priority at all times.
        </p>
        <p class="p-2 text-start">
          We offer over 20 years recruitment experience within the wider
          engineering sector. Our consultants have operated across Power
          Transmission, Drives & Controls, Electrical & Instrumentation,
          Automation and Maintenance.
        </p>
        <p class="p-2 text-start">
          Technical competence, attitude and behavior are all discerning
          qualities in our opinion. We interview our candidates to ensure they
          align to your culture and values. We consider it to be a vital
          component in ensuring a positive recruitment outcome. Promoting your
          business in an attempt to foster the right culture and talent fit is
          something we take pride in.
        </p>
        <p class="p-2 text-start">
          We use realistic business indicators on a daily basis to ensure the
          work we undertake is proactive rather than reactive. Currently 87% of
          the roles we recruit for we deliver on.
        </p>
        <p class="p-2 text-start">
          Providing an exclusive, retained and contingency based service to
          client and candidate alike, all we ask is that you entrust us with
          your needs, both personal and professional.
        </p>
      </div>
      <div class="mx-auto w-full my-10">
        <h3 class="text-red-700 text-center">
          These are the typical roles we cover
        </h3>
        <div class="flex justify-center items-center mt-5">
          <ul class="list-group list-group-flush leading-8">
            <li class="list-group-item">Engineering Manager</li>
            <li class="list-group-item">E&I Engineer</li>
            <li class="list-group-item">Reliability Engineer</li>
            <li class="list-group-item">Multi Skilled Engineer</li>
            <li class="list-group-item">Engineering Coordinator</li>
            <li class="list-group-item">Maintenance Engineer</li>
            <li class="list-group-item">Electrical Maintenance Engineer</li>
            <li class="list-group-item">Design Engineer</li>
            <li class="list-group-item">Mechanical Fitter</li>
            <li class="list-group-item">Sales Engineer</li>
            <li class="list-group-item">Applications Engineer</li>
            <li class="list-group-item">Systems Engineer</li>
            <li class="list-group-item">Instrumentation & Controls Engineer</li>
            <li class="list-group-item">Maintenance Team Leader / Manager</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="border-t w-full mx-auto mt-4">
      <div class="mt-5">
        <h2 class="text-xl text-muted text-center font-bold my-8">
          View our most recent
          <span class="text-blue-600">LinkedIn</span> activity
        </h2>
      </div>
      <div class="bg-blue-600 p-4 mb-3 md:mb-5">
        <swiper
          :slidesPerView="1"
          :spaceBetween="20"
          :slidesPerGroup="1"
          :loop="true"
          :loopFillGroupWithBlank="true"
          class="mySwiper"
          :autoplay="{
            delay: 3500,
            disableOnInteraction: true,
          }"
          :pagination="{
            clickable: true,
          }"
          :modules="modules"
          :breakpoints="{
            '667': {
              slidesPerView: 1,
              spaceBetween: 20,
            },
            '768': {
              slidesPerView: 1,
              spaceBetween: 20,
            },
            '1024': {
              slidesPerView: 3,
              spaceBetween: 20,
              slidesPerGroup: 1,
            },
          }"
        >
          <swiper-slide>
            <a
              href="https://www.linkedin.com/search/results/all/?heroEntityKey=urn%3Ali%3Afsd_profile%3AACoAAA9IA4UBpAT5Vno2hrXoaj2Lnvbwq-8qucI&keywords=mark%20wilson&origin=RICH_QUERY_TYPEAHEAD_HISTORY&position=0&searchId=9b3955a0-8b93-4cb7-a31a-1d585c693281&sid=y4s"
            >
              <div class="w-full">
                <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7021820531779719170" height="350" width="460" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>              </div>
            </a>
          </swiper-slide>
          <swiper-slide>
            <a
              href="https://www.linkedin.com/search/results/all/?heroEntityKey=urn%3Ali%3Afsd_profile%3AACoAAA9IA4UBpAT5Vno2hrXoaj2Lnvbwq-8qucI&keywords=mark%20wilson&origin=RICH_QUERY_TYPEAHEAD_HISTORY&position=0&searchId=9b3955a0-8b93-4cb7-a31a-1d585c693281&sid=y4s"
            >
              <div class="w-full">
                <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7021816226431528960" height="350" width="460" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>             </div>
            </a>
          </swiper-slide>
          <swiper-slide>
            <a
              href="https://www.linkedin.com/search/results/all/?heroEntityKey=urn%3Ali%3Afsd_profile%3AACoAAA9IA4UBpAT5Vno2hrXoaj2Lnvbwq-8qucI&keywords=mark%20wilson&origin=RICH_QUERY_TYPEAHEAD_HISTORY&position=0&searchId=9b3955a0-8b93-4cb7-a31a-1d585c693281&sid=y4s"
            >
              <div class="w-full">
                <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7025463932232302592" height="350" width="460" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>             </div>
            </a>
          </swiper-slide>
          <swiper-slide>
            <a
              href="https://www.linkedin.com/search/results/all/?heroEntityKey=urn%3Ali%3Afsd_profile%3AACoAAA9IA4UBpAT5Vno2hrXoaj2Lnvbwq-8qucI&keywords=mark%20wilson&origin=RICH_QUERY_TYPEAHEAD_HISTORY&position=0&searchId=9b3955a0-8b93-4cb7-a31a-1d585c693281&sid=y4s"
            >
              <div class="w-full">
                <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7025870845164027904" height="350" width="460" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>             </div>
            </a>
          </swiper-slide>
          <swiper-slide>
            <a
              href="https://www.linkedin.com/search/results/all/?heroEntityKey=urn%3Ali%3Afsd_profile%3AACoAAA9IA4UBpAT5Vno2hrXoaj2Lnvbwq-8qucI&keywords=mark%20wilson&origin=RICH_QUERY_TYPEAHEAD_HISTORY&position=0&searchId=9b3955a0-8b93-4cb7-a31a-1d585c693281&sid=y4s"
            >
              <div class="w-full">
                <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7026546690853609472" height="350" width="460" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>            </div>
            </a>
          </swiper-slide>
          <swiper-slide>
            <a
              href="https://www.linkedin.com/search/results/all/?heroEntityKey=urn%3Ali%3Afsd_profile%3AACoAAA9IA4UBpAT5Vno2hrXoaj2Lnvbwq-8qucI&keywords=mark%20wilson&origin=RICH_QUERY_TYPEAHEAD_HISTORY&position=0&searchId=9b3955a0-8b93-4cb7-a31a-1d585c693281&sid=y4s"
            >
              <div class="w-full">
                <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7026852599714738177" height="350" width="460" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>            </div>
            </a>
          </swiper-slide>

        </swiper>
      </div>
    </div>

  </div>
</template>

<script>
import { Navigation, Pagination, Autoplay } from "swiper";
import { Swiper, SwiperSlide } from "swiper/vue";
// Import Swiper styles
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";
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
      console.log("slide change");
    };
    return {
      onSwiper,
      onSlideChange,
      modules: [Navigation, Pagination, Autoplay],
    };
  },
  data() {
    return {};
  },
};
</script>
<style scoped>
/* Extra Small Devices, Phones */
@media only screen and (min-width: 480px) {
}
/* Small Devices, Tablets */
@media only screen and (min-width: 768px) {
}
/* Medium Devices, Desktops */
@media only screen and (min-width: 992px) {
  .about-info {
    border-right: 1px solid red;
    padding-right: 10%;
  }
}
/* Large Devices, Wide Screens */
@media only screen and (min-width: 1200px) {
}
</style>