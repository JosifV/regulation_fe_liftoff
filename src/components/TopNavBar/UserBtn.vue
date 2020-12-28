<template>
   <v-menu offset-y >
      <template v-slot:activator="{ on, attrs }">
        <v-btn class="user_cont"
          v-bind="attrs"
          v-on="on"
          :elevation="0"
        >
          <v-icon :color="colors.primary" dark size="50"> mdi-account-circle </v-icon>
        </v-btn>
      </template>
      <v-list>
        <v-list-item
          v-for="(item, index) in 4"
          :key="index"
        >
          <v-list-item-title>{{ item }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
</template>

<script lang="ts">
import {COLORS} from '../../const'

export default {
  name: "UserBtn",
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
