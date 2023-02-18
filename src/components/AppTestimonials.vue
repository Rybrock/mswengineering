    <template>
  <div class="w-full p-5" id="testimonials">
    <div class="w-full h-full mx-auto p-2">
      <div class="mb-2">
        <h2 class="text-center mb-10 text-2xl">Recent Testimonials</h2>
      </div>
      <swiper
        :slidesPerView="1"
        :spaceBetween="10"
        :slidesPerGroup="1"
        :loop="true"
        class="mySwiper"
        :centered-slides="true"
        :autoplay="{
          delay: 3500,
          disableOnInteraction: true,
        }"
        :pagination="{
          clickable: true,
        }"
        :modules="modules"
        :navigation="false"
        :breakpoints="{
          '667': {
            slidesPerView: 1,
            spaceBetween: 50,
          },
          '768': {
            slidesPerView: 1,
            spaceBetween: 40,
          },
          '1024': {
            slidesPerView: 3,
            spaceBetween: 50,
            slidesPerGroup: 1,
          },
        }"
      >
        <swiper-slide v-for="(item, index) in testimonials" :key="index">
          <div class="card w-full text-center p-4 border">
            <div class="card-body w-full">
              <h5 class="card-title text-red-700 font-bold">
                {{ item.title }}
              </h5>
              <h6 class="card-subtitle mb-2 font-bold text-red-700">
                {{ item.subtitle }}
              </h6>
              <p class="card-text w-full mt-2">
                {{ item.text }}
              </p>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>
  <script>
// Import Swiper Vue.js components
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
  data() {
    return {
      testimonials: [
      {
          subtitle: "Automation Engineer",
          date: "Nov 26, 2022",
          text: "Mark helped in getting a job in a company which suited all my needs and helped answer any and all questions I had. He was constantly in touch and ready to help whenever I needed him. The company is an amazing fit and I wouldn’t have found it otherwise.",
        },
        {
          subtitle: "Facilities Engineer",
          date: "Nov 2, 2022",
          text: "Had a great experience with Mark and my job hunt. Went above and beyond to ensure all the boxes were ticked. Out of hours calls, genuine pros and cons conversations with respect to my situation and no pushing for personal benefit or gain. Would recommend to fellow engineers in there hunt for new jobs.",
        },
        {
          subtitle: "Multi skilled Engineer",
          date: "August 20, 2022",
          text: "Great service from Mark. I was given all the information about the role and was contacted every step of the way. Mark really made an effort and did everything he said he would.",
        },
        {
          subtitle: "Engineering Supervisor",
          date: "September 8, 2022",
          text: "Mark's been great in finding me my new job role and has always been there to answer any of my questions along the way would definitely recommend him for anyone looking for work.",
        },
        {
          subtitle: "Engineering Manager",
          date: "August 12, 2022",
          text: "A pleasure to deal with, didn't leave me with any of the questions that most recruiters do. If you had a question/query he would be straight back to you as soon as humanly possible.",
        },
        {
          subtitle: "Equipment Engineer",
          date: "July 16, 2022",
          text: "During my job search, it was Mark's main focus to find me the role that I would be happiest and most successful in. He was very helpful with preparing for the interviews which he facilitated and nothing was too much trouble.",
        },
        {
          subtitle: "Electrical Engineer",
          date: "June 20, 2022",
          text: "Great recruiter and really helpful, always available and has the information you need to know and will always get back to you straight away with any questions you have. ",
        },
        {
          subtitle: "Multi-skilled Maintenance Engineer",
          date: "June 20, 2022",
          text: "Although I didn't end up taking a job that had been set up by Mark, we built a fantastic working relationship throughout the process where he supported me with interview advice and career guidance until the very end.",
        },
        {
          subtitle:
            "Senior Leader | Catalyst for change | Cross Functional Alignment",
          date: "December 5, 2019",
          text: "Since Mark placed me in a previous role.. he has not just been a recruitment consultant he's been a friend that iv kept in touch with. Always on hand to speak to and interested in not just placing me but me as a person. fantastic professional guy.",
        },
        {
          subtitle: "Site Engineer",
          date: "June 25, 2019",
          text: "Mark is superb example of understanding the requirements of what is required by both parties. He is a dedicated professional and supplies excellent communication with regular updates.",
        },
        {
          subtitle: "Site Engineering Manager",
          date: "June 9, 2015",
          text: "Mark understands the needs of both; the potential Employer and the Employee. He is detailed in his approach and ensures 'follow up' and communication are at the forefront.",
        },
      ],
    };
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
};
</script>
<style>
h6.card-subtitle {
  font-size: 0.75rem !important;
}
p.card-text {
  font-size: 0.8rem !important;
}
.swiper-pagination {
  position: relative;
  bottom: 10px;
  padding: 20px !important;
  width: 100%;
}
div.card {
  height: 200px;
}
#testimonials {
  margin-top: 1rem !important;
}
@media only screen and (max-width: 600px) {
  div.card {
  height: 290px;
}
}
</style>