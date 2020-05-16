<template>
  <div style="height:100vh">
    <Evaluation class="mb-5"></Evaluation>
    <v-card class="mb-5" style="height:30%">
      <v-card-title>Team Notes</v-card-title>
      <v-text>
        <v-list>
          <v-list-item>
            <v-list-item-avatar color="primary" size="36">
              <span class="white--text headline pl-1">VJ</span>
            </v-list-item-avatar>

            <v-list-item-title>
              Task
              <span style="color:#555;font-size:0.8rem">2:30 pm</span>
              <br />
              <span
                class="text--secondary"
              >Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia, sunt fugiat. Voluptate ducimus numquam, tempore tenetur quasi eligendi expedita, provident quam ex modi quibusdam nobis corrupti velit saepe explicabo quia.</span>
            </v-list-item-title>
          </v-list-item>
          <v-divider></v-divider>
          <v-list-item>
            <v-list-item-avatar color="primary" size="36">
              <span class="white--text headline pl-1">VJ</span>
            </v-list-item-avatar>

            <v-list-item-title>
              Task
              <span style="color:#555;font-size:0.8rem">2:30 pm</span>
              <br />
              <span
                class="text--secondary"
              >Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia, sunt fugiat. Voluptate ducimus numquam, tempore tenetur quasi eligendi expedita, provident quam ex modi quibusdam nobis corrupti velit saepe explicabo quia.</span>
            </v-list-item-title>
          </v-list-item>
          <v-divider></v-divider>
        </v-list>
      </v-text>
    </v-card>
    <v-card class="mb-5" style="height:30%">
      <v-card-title>Team Notes</v-card-title>
      <v-text>hello</v-text>
    </v-card>
    <v-space></v-space>
  </div>
</template>

<script>
import Evaluation from "./RightNavComponents/Evaluation";
export default {
  name: "RightComp",
  components: { Evaluation }
};
</script>

<style>
</style>