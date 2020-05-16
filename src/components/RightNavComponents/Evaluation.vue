<template>
  <v-card>
    <v-card-text>
      <span>Evaluation</span>
      <v-btn color="primary" text>
        <v-icon>mdi-calendar</v-icon>Schedule
      </v-btn>
      <v-btn text>
        <v-icon>mdi-share-variant</v-icon>
      </v-btn>
      <v-btn text>
        <v-icon>mdi-telegram</v-icon>
      </v-btn>
      <v-btn color="primary" text>More</v-btn>
    </v-card-text>
    <v-divider></v-divider>
    <v-card-text>
      <span>Job Name</span>
      <v-btn color="primary" text>
        <v-icon>mdi-check</v-icon>Proceed
      </v-btn>
      <v-btn color="primary" text>
        <v-icon>mdi-cancel</v-icon>
      </v-btn>
      <v-btn color="primary" text>
        <v-icon>mdi-dots-horizontal</v-icon>
      </v-btn>
    </v-card-text>
    <v-divider></v-divider>
    <v-card-text>
      <span>Pool Name</span>
      <v-btn color="primary" text>
        <v-icon>mdi-check</v-icon>Proceed
      </v-btn>
      <v-btn color="primary" text>
        <v-icon>mdi-cancel</v-icon>
      </v-btn>
      <v-btn color="primary" text>
        <v-icon>mdi-dots-horizontal</v-icon>
      </v-btn>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: "Evaluation"
};
</script>

<style>
</style>