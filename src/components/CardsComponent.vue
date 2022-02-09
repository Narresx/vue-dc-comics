<template>
  <div>
    <div class="container-jumbo"></div>
    <div class="container-cards">
      <div class="container-comic d-flex">
        <div class="comic-card">
          <img :src="thumb" :alt="type" />
          <h2 class="text-white">
            {{ series }}
          </h2>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardsComponent",
  props: ["thumb", "series", "type"],
};
</script>

<style lang="scss" scoped>
.text-white {
  color: white;
}

.d-flex {
  display: flex;
}

.container-jumbo {
  width: 100%;
  height: 450px;
  background-image: url("../assets/img/jumbotron.jpg");
}

.container-cards {
  width: 100%;
  height: auto;
}

.container-comic {
  margin: 0 auto;
  width: 800px;
  height: auto;
}

.comic-card {
  flex-basis: calc(100 / 6) -5px;
  padding: 5px;
}
</style>