<template>
  <v-container>
    <v-row class="text-center">
      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          E-Mobility Behaviour
        </h1>
      </v-col>

      <v-col class="mb-5" cols="12">
        <v-card elevation="5">
          <v-card-title>Dummy Plot</v-card-title>
          <v-card-text>
            <Plotly
              :data="datapoints"
              :layout="layout"
              :display-mode-bar="false"
            ></Plotly>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { Plotly } from "vue-plotly";

export default {
  name: "HelloWorld",
  components: {
    Plotly,
  },
  data: function() {
    return {
      datapoints: [{ x: [1, 3], y: [2, 4] }],
      layout: {},
      options: {},
    };
  },
};
</script>
