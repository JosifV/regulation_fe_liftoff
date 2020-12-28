<template>
  <div class="top_navbar_cont">
    <HomeBtn />
    <Documents />
    <UserBtn />
  </div>
</template>

<script lang="ts">
import HomeBtn from "./TopNavBar/HomeBtn.vue";
import UserBtn from "./TopNavBar/UserBtn.vue";
import Documents from "./TopNavBar/Documents.vue";

import { COLORS } from "../const";

export default {
  name: "TopNavBar",
  components: {
    HomeBtn,
    UserBtn,
    Documents,
  },
  data() {
    return {
      colors: COLORS,
    };
  },
};
</script>

<style>
</style>
