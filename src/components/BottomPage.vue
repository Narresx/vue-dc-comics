<template>
  <div>
    <div
      class="d-flex container space-between space-align-center background-gray"
    >
      <div class="text-white">
        <a href="#"
          ><button class="button-style text-white">SIGN-UP NOW!</button></a
        >
      </div>
      <div class="d-flex space-align-center">
        <div class="d-flex space-between">
          <h2 class="text-blue">FOLLOW US</h2>
          <figure v-for="card in cards" :key="card.url" class="paddig-icons">
            <img :src="require(`../assets/img/${card.url}`)" />
          </figure>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomPage",

  data() {
    return {
      cards: [
        { url: "footer-facebook.png" },
        { url: "footer-twitter.png" },
        { url: "footer-youtube.png" },
        { url: "footer-pinterest.png" },
        { url: "footer-periscope.png" },
      ],
    };
  },
};
</script>

<style>
.background-gray {
  background-color: rgb(48, 48, 48);
  z-index: 2;
  height: 100px;
}

.paddig-icons {
  padding-left: 15px;
}

.d-flex {
  display: flex;
}

.space-between {
  justify-content: space-between;
}

.space-align-center {
  align-items: center;
}

.button-style {
  border: 3px solid rgb(2, 130, 249);
  padding: 15px 25px;
  background-color: transparent;
}

.text-white {
  color: white;
}

.text-blue {
  color: rgb(2, 130, 249);
}

.container {
  width: 100%;
  height: 100px;
}
</style>