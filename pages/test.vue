<template>
  <div>
    <!-- v-if とその仲間たち -->
    <div v-if="score >= 80">よくできました</div>
    <div v-else-if="score >= 30">もっといける！！</div>
    <div v-else>がんばろう！</div>

    <a :href="googleLink">Googleへのリンク</a>
    <img
      src="https://2.bp.blogspot.com/-zDsrPiqkR_0/U0pTNj7lpoI/AAAAAAAAfGA/2Z1onz10tAw/s800/grade2_yokudekimashita.png"
      alt="よくできました"
    />

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
      googleLink: 'https://google.com',
    }
  },
  methods: {
    toggleShown() {
      this.isShown = !this.isShown
    },
  },
}
</script>
