<template>
  <div>
    <div class="background-gray text-white">
      <a href="#"
        ><button class="button-style text-white">SIGN-UP NOW!</button></a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomPage",
};
</script>

<style>
.background-gray {
  background-color: rgb(48, 48, 48);
  z-index: 2;
  height: 100px;
}

.d-flex {
  display: flex;
}

.button-style {
  border: 3px solid rgb(2, 130, 249);
  padding: 15px 25px;
  background-color: transparent;
}

.text-white {
  color: white;
}
</style>