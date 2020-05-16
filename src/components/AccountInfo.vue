<template>
  <v-container>
    <v-row>
      <v-col cols="1"></v-col>
      <v-col cols="2" style="z-index:0">
        <v-avatar height="100%" width="100%">
          <img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="John" />
        </v-avatar>
      </v-col>
      <v-col cols="9" class="pl-5 pt-5">
        <v-row>
          <p class="display-3">{{Name}}</p>
        </v-row>
        <v-row>
          <p class="display-1 text--secondary">{{Designation}}</p>
        </v-row>
        <v-row>
          <p class="display-1 text--secondary">{{lastActive}}</p>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "AccountInfo",
  data() {
    return {
      Name: "Kunal",
      Designation: "Full Stack",
      lastActive: "Online"
    };
  }
};
</script>

<style>
</style>