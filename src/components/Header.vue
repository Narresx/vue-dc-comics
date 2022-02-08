<template>
  <header>
    <nav>
      <figure>
        <img src="../assets/img/dc-logo.png" alt="Logo dc" />
      </figure>
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url" :class="{ active: link.active }">{{
            link.text
          }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script scoped>
export default {
  name: "Header",
  data() {
    return {
      links: [
        { text: "CHARACTER", url: "#", active: false },
        { text: "COMICS", url: "#", active: false },
        { text: "MOVIES", url: "#", active: false },
        { text: "TV", url: "#", active: false },
        { text: "GAMES", url: "#", active: false },
        { text: "COLLECTIBLES", url: "#", active: false },
        { text: "VIDEOS", url: "#", active: false },
        { text: "FANS", url: "#", active: false },
        { text: "NEWS", url: "#", active: false },
        { text: "SHOP", url: "#", active: false },
      ],
    };
  },
};
</script>

<style scoped>
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
}

li a:hover,
li a.active {
  color: blue;
}
</style>