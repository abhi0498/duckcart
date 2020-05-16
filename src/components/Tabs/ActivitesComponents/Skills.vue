<template>
  <v-card>
    <v-card-title primary-title>
      <v-row>
        <v-col cols="10">Skills</v-col>
        <v-col cols="1">
          <v-btn @click="enter=!enter" fab small elevation="2" class="align-self-end" color="white">
            <v-icon>mdi-plus</v-icon>
          </v-btn>
        </v-col>
      </v-row>
      <v-card-text class="pl-0 ml-0">
        <v-row v-if="enter">
          <v-col cols="10">
            <v-text-field label="Add Skill" v-model="skill" hide-details="auto"></v-text-field>
          </v-col>
          <v-col cols="2">
            <v-btn class="mt-3" @click="addSkill()">Add</v-btn>
          </v-col>
        </v-row>
        <v-chip
          v-for="(item,index) in skills"
          :key="index"
          class="ma-2"
          color="#2962FF"
          text-color="white"
        >{{item}}</v-chip>
      </v-card-text>
    </v-card-title>
  </v-card>
</template>

<script>
export default {
  name: "SkillCard",
  data() {
    return {
      enter: false,
      skill: "",
      skills: ["web", "react", "vue", "python"]
    };
  },
  methods: {
    addSkill() {
      this.skills = [...this.skills, this.skill];
      this.skill = "";
      this.enter = false;
    }
  }
};
</script>

<style>
</style>