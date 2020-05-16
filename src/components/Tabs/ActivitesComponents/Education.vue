<template>
  <v-card>
    <v-card-title primary-title>
      <v-row>
        <v-col cols="10">Education</v-col>
        <v-col cols="1">
          <v-btn fab small elevation="2" class="align-self-end" color="white">
            <v-icon>mdi-plus</v-icon>
          </v-btn>
        </v-col>
      </v-row>
    </v-card-title>

    <v-card-text>
      <span class="headline">{{education.name}}</span>
      <br />
      {{education.place}}
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: "EducationCard",
  data() {
    return {
      education: {
        name: "SSC",
        place: "HH HS",
        gradDate: "SEP 2016",
        remarks: "CGPA: 7.5"
      }
    };
  }
};
</script>

<style>
</style>