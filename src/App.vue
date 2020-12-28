<template>
  <v-app>
    <div class="top_level_cont">
      <div class="top_navbar_wrap">
        <TopNavBar />
      </div>
      <div class="main_view_wrap">
        <Sidebar />
        <MainView />
      </div>
    </div>
  </v-app>
</template>

<script>
import TopNavBar from "./components/TopNavBar.vue";
import Sidebar from "./components/Sidebar.vue";
import MainView from "./components/MainView.vue";

export default {
  name: "App",
  components: {
    TopNavBar,
    Sidebar,
    MainView,
  },
};
</script>

<style lang="scss">
@import url("./style/index.scss");
</style>