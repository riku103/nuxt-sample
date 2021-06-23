<template>
  <div>
    <div v-show="isShown">みえるかな？</div>
    <v-btn @click="toggleShown">表示/非表示の切り替え</v-btn>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isShown: true,
    }
  },
  methods: {
    toggleShown() {
      this.isShown = !this.isShown
    },
  },
}
</script>
