<template>
  <div>
    <nav class="p-5">
      <div class="nav-wrapper place-items-center space-x-6 w-full flex">
        <div class="px-0 md:px-5 flex flex-col md:flex-row justify-around items-center space-x-10">
          <div class="md:hidden flex justify-start items-start w-full" @click.prevent="openCloseNav()">
            <div>
              <img src="../assets/menu_FILL0_wght400_GRAD0_opsz48.svg" width="30" height="30" alt="menu icon" class="top-0" />
            </div>
          </div>
          <div class="logo">
            <router-link class="navbar-brand" to="/">
              <img
                src="../assets/MSW_TW-1647012258new.png"
                alt=""
                class="w-100"
              />
            </router-link>
          </div>
          <div class="space-x-8 hidden md:flex">
            <router-link to="/" class="p-2 rounded-lg hover:bg-red-700 hover:text-white">Home</router-link>
            <router-link to="/about" class="p-2 rounded-lg hover:bg-red-700 hover:text-white">About</router-link>
          </div>
        </div>
      </div>
      <div
        v-if="navIsOpen"
        class="nav-modal shadow-lg absolute top-5 left-0 bg-white p-4 w-10/12"
      >
        <div class="top-0 right-5">
          <img @click.prevent="openCloseNav()" src="../assets/close_FILL0_wght400_GRAD0_opsz48.svg" width="20"
                      height="20" alt="close menu icon" class="font-bold">
        </div>
        <div class="text-xl p-4">
          <ul class="space-y-8">
            <li @click="openCloseNav()">
              <router-link to="/"> Home </router-link>
            </li>
            <li @click="openCloseNav()">
              <router-link to="/about"> About </router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navIsOpen: false,
    };
  },
  methods: {
    openCloseNav() {
      this.navIsOpen = !this.navIsOpen;
    },
  },
};
</script>

<style scoped>
  div.logo img {
    width: 100%;
    height: 140px !important;
  }
  @media only screen and (max-width: 600px) {
    #app-navbar {
    font-size: 0.5rem !important;
  }
  div.logo img {
    width: 100% !important;
    max-width: 400px !important;
    height: 100px !important;
    padding: 0;
    margin: 0;
  }
  .logo {
    margin-left: 0 !important;
  }

}
</style>