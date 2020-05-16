<template>
  <v-container>
    <InformationCard class="mt-5"></InformationCard>
    <ExperienceCard class="mt-5"></ExperienceCard>

    <v-row class="mt-5">
      <v-col>
        <EducationCard></EducationCard>
      </v-col>

      <v-col>
        <SkillCard></SkillCard>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import InformationCard from "./ActivitesComponents/Information";
import ExperienceCard from "./ActivitesComponents/Experience";
import SkillCard from "./ActivitesComponents/Skills";
import EducationCard from "./ActivitesComponents/Education";
export default {
  name: "Activities",
  components: { InformationCard, ExperienceCard, SkillCard, EducationCard },
  data() {
    return {
      experience: [{}]
    };
  }
};
</script>

<style>
</style>