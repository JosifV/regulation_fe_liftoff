<template>
  <div class="documents_cont">
    <v-sheet class="mx-auto documents_slide">
      <v-slide-group multiple show-arrows>
        <v-slide-item v-for="(n, ind) in 5" :key="`Regulation ${ind}`" v-slot="{ active, toggle }">
          <v-btn
            class="mx-2"
            :input-value="active"
            :active-class="active_class_calc"
            depressed
            @click="toggle"
          >
            Regulation {{ n }}
          </v-btn>
        </v-slide-item>

        <v-divider vertical></v-divider>

         <v-slide-item v-for="(n, ind) in 4" :key="`ASPICE ${ind}`" v-slot="{ active, toggle }">
          <v-btn
            class="mx-2"
            :input-value="active"
            :active-class="active_class_calc"
            depressed
            @click="toggle"
          >
            ASPICE {{ n }}
          </v-btn>
        </v-slide-item>

        <v-divider vertical></v-divider>

        <v-slide-item v-for="(n, ind) in 5" :key="`ISO ${ind}`" v-slot="{ active, toggle }">
          <v-btn
            class="mx-2"
            :input-value="active"
            :active-class="active_class_calc"
            depressed
            @click="toggle"
          >
            ISO {{ n }}
          </v-btn>
        </v-slide-item>

        <v-divider vertical></v-divider>

        <v-slide-item v-for="(n, ind) in 2" :key="`VW ${ind}`" v-slot="{ active, toggle }">
          <v-btn
            class="mx-2"
            :input-value="active"
            :active-class="active_class_calc"
            depressed
            @click="toggle"
          >
            VW {{ n }}
          </v-btn>
        </v-slide-item>
      </v-slide-group>
    </v-sheet>
  </div>
</template>

<script lang="ts">
import { COLORS } from "../../const";

export default {
  name: "Documents",
  components: {},
  data: function () {
    return {
      colors: COLORS,
      active_class_calc: `primary white--text`,
    };
  },
};
</script>

<style>
</style>
