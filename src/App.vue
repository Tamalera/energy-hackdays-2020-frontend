<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      Energy Hackdays 2020
      <v-spacer></v-spacer>
      <v-btn
      class="mr-2"
      ><router-link to="/">Public Charging Stations</router-link></v-btn>
      <v-btn><router-link to="/private">Private Charging Stations</router-link></v-btn>
    </v-app-bar>

    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: "App",

  components: {
  },

  data: () => ({
    //
  }),
};
</script>
