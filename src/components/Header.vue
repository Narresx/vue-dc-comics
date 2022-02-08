<template>
  <header>
    <nav>
      <figure>
        <img src="@/assets/img/dc-logo.png" alt="Logo dc" />
      </figure>
      <ul>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
        <li><a href="#">CHARACTER</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
nav {
  display: flex;
  justify-content: space-between;
}

ul {
  display: flex;
  list-style-type: none;
  justify-content: center;
  align-items: center;
}

li a {
  text-decoration: none;
  padding: 0 10px;
  color: black;
  font-weight: bolder;
  position: relative;
}

li a:hover {
  color: blue;
}
</style>