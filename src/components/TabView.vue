<template>
  <v-tabs grow>
    <v-tabs-slider></v-tabs-slider>

    <v-tab>Overview</v-tab>
    <v-tab-item>
      <v-card flat tile>
        <v-card-text>text</v-card-text>
      </v-card>
    </v-tab-item>

    <v-tab>Activities</v-tab>
    <v-tab-item>
      <Activities style="width:90%"></Activities>
    </v-tab-item>

    <v-tab>Assesments</v-tab>
    <v-tab-item>
      <v-card flat tile>
        <v-card-text>text 2</v-card-text>
      </v-card>
    </v-tab-item>

    <v-tab>Files</v-tab>
    <v-tab-item>
      <v-card flat tile>
        <v-card-text>text 2</v-card-text>
      </v-card>
    </v-tab-item>

    <v-tab>Resume</v-tab>
    <v-tab-item>
      <v-card flat tile>
        <v-card-text>text 2</v-card-text>
      </v-card>
    </v-tab-item>
  </v-tabs>
</template>

<script>
import Activities from "./Tabs/Activities";
export default {
  name: "TabView",
  components: {
    Activities
  }
};
</script>

<style>
</style>