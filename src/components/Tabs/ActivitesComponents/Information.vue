<template>
  <v-card outlined height="300">
    <v-card-title primary-title>
      <v-row>
        <v-col cols="11">Information</v-col>
        <v-col cols="1">
          <v-btn fab small elevation="2" class="align-self-end" color="white">
            <v-icon>mdi-plus</v-icon>
          </v-btn>
        </v-col>
      </v-row>
    </v-card-title>
    <!-- <v-list>
        <v-list-item>
          <v-list-item-content>
            <p style="font-size:32px">Information</p>
          </v-list-item-content>
          <v-list-item-icon>
            <v-btn fab small elevation="2" color="white">
              <v-icon>mdi-plus</v-icon>
            </v-btn>
          </v-list-item-icon>
        </v-list-item>

        <v-list-item>
          <v-list-item-content>
            <p>
              Email
              <span style="padding-left:100px">a@a.com</span>
            </p>
          </v-list-item-content>
        </v-list-item>
    </v-list>-->

    <v-simple-table>
      <template v-slot:default>
        <tbody style="padding:10px">
          <tr v-for="item in personalDetails" :key="item.name">
            <td width="20%">{{ item.name }}</td>
            <td width="75%" style="text-align:left">{{ item.values }}</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
  </v-card>
</template>

<script>
export default {
  name: "InformationCard",
  data() {
    return {
      personalDetails: [
        {
          name: "EMAIL",
          values: "aguy@gmail.com"
        },
        {
          name: "PHONE",
          values: "237-908-999"
        },
        {
          name: "SOCIAL",
          values: "github.com/abhi0498"
        },
        {
          name: "LINKS",
          values: "codepen.io"
        }
      ]
    };
  }
};
</script>

<style>
</style>