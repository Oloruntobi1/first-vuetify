<template>
  <!-- <v-card :color="color" dark>
    <v-card-text>
      <v-sparkline
        :value="sales"
        :labels="labels"
        :color="color"
        height="100"
        padding="24"
        stroke-linecap="round"
        smooth
      />
    </v-card-text>

    <v-card-text class="text-center">
      <div class="display-1">{{ title }}</div>
    </v-card-text>
  </v-card> -->
  <v-card :color="sale.color" dark>
    <v-card-text>
      <v-sparkline
        :value="sale.sales"
        :labels="sale.labels"
        color="rgba(255, 255, 255, .7)"
        height="100"
        padding="24"
        stroke-linecap="round"
        smooth
      />
    </v-card-text>

    <v-card-text class="text-center">
      <div class="display-1">{{ sale.title }}</div>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'SalesGraph',
  props: {
    // title: {
    //   type: Object,
    //   required: true
    // },
    sale: {
      type: Object,
      required: true
    }
    // ,
    // color: {
    //   type: Object,
    //   required: true
    // },
    // labels: {
    //   type: Object,
    //   required: true
    // },
  }
}
</script>