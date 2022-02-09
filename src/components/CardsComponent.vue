<template>
  <div class="comic-card">
    <img :src="thumb" :alt="type" />
    <h2 class="text-white">
      {{ series }}
    </h2>
  </div>
</template>

<script>
export default {
  name: "CardsComponent",
  props: ["thumb", "series", "type"],
};
</script>

<style lang="scss" scoped>
.comic-card {
  flex-basis: calc(100% / 6);
  justify-content: center;
  align-items: center;
}

.comic-card img {
  width: 200px;
  height: 200px;
}
</style>