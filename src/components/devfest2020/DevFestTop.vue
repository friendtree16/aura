<template>
  <!-- <v-container class="pa-0"> -->
  <v-layout wrap align-center justify-center row fill-height class="pb-4">
    <v-img
      src="/img/devfest2020/topimg.jpg"
      lazy-src="/img/devfest2020/topimg.jpg"
      alt="GDG DevFest 2020"
      width="100%"
    >
      <v-layout slot="placeholder" fill-height align-center justify-center ma-0>
        <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
      </v-layout>
      <v-layout wrap align-end justify-center row fill-height class="pb-4">
        <div>
          <v-btn
            :href="devfestDetails.EntryPageUrl"
            class="pa-4 ma-4 elevation-0 hidden-sm-and-down"
            target="_blank"
            color="#1705df"
            style="font-size:150%; text-transform: capitalize; border-radius:0px; border: 8px solid white; color:white"
          >Register now</v-btn>
        </div>
      </v-layout>
    </v-img>
    <v-flex xs12 sm4 text-xs-center>
      <div>
        <v-btn
          :href="devfestDetails.EntryPageUrl"
          class="pa-4 ma-4 elevation-0 hidden-md-only hidden-lg-and-up"
          target="_blank"
          color="#1705df"
          style="font-size:150%; text-transform: capitalize; border-radius:0px; border: 5px solid white; color:white"
        >Register now</v-btn>
      </div>
      <!-- <br />
      <div>
        <v-btn
          :href="devfestDetails.PamphletUrl"
          class="pa-5 ma-0 google-font elevation-1"
          target="_blank"
          color="#1a73e8"
          style="font-size:150%; text-transform: capitalize; border-radius:5px; color:white"
        >パンフレット<br />(Pamphlet)</v-btn>
      </div>-->
    </v-flex>
  </v-layout>
  <!-- </v-container> -->
</template>

<script>
import DevFestDetails from "@/assets/data/devfest2020.json";
import Mixin from "@/mixin.js";
export default {
  data() {
    return {
      devfestDetails: DevFestDetails,
    };
  },
  mixins: [Mixin],
};
</script>
