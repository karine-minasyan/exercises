<template>
  <v-container>
    <v-btn cols="12" :color="color" @click="increase()">Button<slot></slot></v-btn> {{ counter }}
  </v-container>
</template>

<script>
export default {
  data: () => ({
    counter: 0
  }),
  methods: {
    increase: function () {
      this.counter++
    }
  },
  props: {
    color: String
  }
}
</script>
