<template>
  <v-btn class="home_cont">
      <v-icon :color="colors.primary" dark size="50" :elevation="0"> mdi-home </v-icon>
    </v-btn>
</template>

<script lang="ts">
import {COLORS} from '../../const'

export default {
  name: "HomeBtn",
  components: {},
  data(){
    return{
      colors: COLORS
    }
  }
};
</script>

<style>
</style>
