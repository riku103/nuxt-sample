<template>
  <div class="container">
    <div class="number">{{ count }}</div>
    <v-btn class="mx-1" fab dark color="blue" @click="plus">
      <v-icon dark> mdi-plus </v-icon>
    </v-btn>
    <v-btn class="mx-1" fab dark color="orange" @click="minus">
      <v-icon dark> mdi-minus </v-icon>
    </v-btn>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 100,
    }
  },
  methods: {
    plus() {
      this.count += 1
    },
    minus() {
      this.count -= 1
    },
  },
}
</script>

<style lang="scss">
.container {
  .number {
    font-size: 64px;
  }
}
</style>
