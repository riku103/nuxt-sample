<template>
  <div>
    <div>テスト</div>

    <v-text-field ref="number" v-model="number" />
    <div>数値: {{ number }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number: 0,
    }
  },

  created() {
    console.log('created')
  },

  mounted() {
    console.log('mounted')
    this.$refs.number.focus()
  },

  updated() {
    console.log('updated')
    console.log(this.number)
  },
}
</script>

<style lang="scss" module></style>
