<template>
  <v-app>
    <!-- <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn href="https://github.com/vuetifyjs/vuetify/releases/latest" target="_blank" text>
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>-->

    <v-content>
      <div>
        <v-row style="position:sticky;top:0;left:0">
          <v-col cols="1">
            <v-btn elevation="0" color="white" @click.stop="drawer = !drawer">
              <v-icon>mdi-menu</v-icon>
            </v-btn>
          </v-col>
          <v-col style="text-align:center" cols="10">Employee/Profile</v-col>
          <v-col cols="1">Back</v-col>
        </v-row>

        <v-navigation-drawer style="height:100vh" v-model="drawer" absolute temporary>
          <v-list-item>
            <v-btn elevation="0" color="white" @click.stop="drawer = !drawer">
              <v-icon>mdi-menu</v-icon>
            </v-btn>

            <v-list-item-content class="px-3">
              <v-list-item-title>INGOIT</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          <v-divider></v-divider>

          <v-list dense>
            <v-list-item v-for="item in items" :key="item.title" link>
              <v-list-item-icon>
                <v-icon>{{ item.icon }}</v-icon>
              </v-list-item-icon>

              <v-list-item-content>
                <v-list-item-title>{{ item.title }}</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-navigation-drawer>
      </div>
      <v-container>
        <v-row>
          <v-col cols="9">
            <AccountInfo></AccountInfo>
            <TabView></TabView>
          </v-col>

          <v-col style="position:fixed;right:0" cols="3">
            <RightComp></RightComp>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>


<script>
// import NavDrawer from "./components/NavDrawer";
import AccountInfo from "./components/AccountInfo";
import TabView from "./components/TabView";
import RightComp from "./components/RightComp";

export default {
  name: "App",

  components: {
    RightComp,
    AccountInfo,
    TabView
  },

  data() {
    return {
      drawer: null,
      items: [
        { title: "Dashboard", icon: "mdi-view-dashboard" },
        { title: "Candidates", icon: "mdi-account-multiple" },
        { title: "Jobs", icon: "mdi-briefcase" },
        { title: "Mailbox", icon: "mdi-email" },
        { title: "Settings", icon: "mdi-settings-box" }
        // { title: "Pools", icon: "question_answer" },
        // { title: "Assesments", icon: "dashboard" },
        // { title: "Team Members", icon: "question_answer" }
      ]
    };
  }
};
</script>
