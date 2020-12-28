<template>
  <div class="sidebar_cont">
    <!--  -->

    <v-expansion-panels>
    <v-expansion-panel
      v-for="(item,i) in 7"
      :key="i"
    >
      <v-expansion-panel-header>
        Sec {{item}}
      </v-expansion-panel-header>
       <v-divider></v-divider>
      <v-expansion-panel-content>

        <v-list nav dense>
        <v-list-item link>
          <v-list-item-icon>
            {{item}}.1
          </v-list-item-icon>
        </v-list-item>
        <v-list-item link>
          <v-list-item-icon>
            {{item}}.2
          </v-list-item-icon>
        </v-list-item>
        <v-list-item link>
          <v-list-item-icon>
            {{item}}.3
          </v-list-item-icon>
        </v-list-item>
      </v-list>

      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>

  </div>
</template>

<script lang="ts">
export default {
  name: "Sidebar",
  components: {},
};
</script>

<style>
</style>
