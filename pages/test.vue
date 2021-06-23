<template>
  <div>
    <!-- v-if とその仲間たち -->
    <div v-if="score >= 80">よくできました</div>
    <div v-else-if="score >= 30">もっといける！！</div>
    <div v-else>がんばろう！</div>

    <!-- v-show -->
    <!-- <div v-show="isShown">みえるかな？</div> -->
    <!-- <v-btn @click="toggleShown">表示/非表示の切り替え</v-btn> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      isShown: true,
      score: 90,
    }
  },
  methods: {
    toggleShown() {
      this.isShown = !this.isShown
    },
  },
}
</script>
