<template>
  <main>
    <section class="container background-black">
      <div class="text-white">Content goes here</div>
    </section>
    <section class="container background-lightblue d-flex text-white">
      <nav>
        <figure>
          <img src="../assets/img/buy-comics-digital-comics.png" />
          <div>DIGITAL COMICS</div>
        </figure>
        <figure>
          <img src="../assets/img/buy-comics-merchandise.png" />
          <div>DC MERCHANDISE</div>
        </figure>
        <figure>
          <img src="../assets/img/buy-comics-subscriptions.png" />
          <div>SUBSCRIPTION</div>
        </figure>
        <figure>
          <img src="../assets/img/buy-comics-shop-locator.png" />
          <div>COMIC SHOP LOCATOR</div>
        </figure>
        <figure>
          <img src="../assets/img/buy-dc-power-visa.svg" />
          <div>DC POWER VISA</div>
        </figure>
      </nav>
    </section>
  </main>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style scoped>
.container {
  margin: 0 auto;
  max-width: 100%;
}

.text-white {
  color: white;
}

.background-black {
  background-color: black;
}
.background-lightblue {
  background-color: rgb(2, 130, 249);
}

nav,
figure {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

section figure img {
  width: 65px;
  height: 65px;
}

figure div {
  padding-left: 10px;
}

.d-flex {
  display: flex;
}

section {
  height: 250px;
}
</style>