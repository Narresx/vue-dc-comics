<template>
  <footer class="d-flex">
    <section class="d-flex f-wrap">
      <nav class="margin-top d-flex d-column">
        <h2 class="text-white margin-right">DC COMICS</h2>
        <ul>
          <li v-for="(link, index) in links1" :key="index">
            <a :href="link.url" :class="{ active: link.active }">{{
              link.text
            }}</a>
          </li>
        </ul>
      </nav>
      <nav class="margin-top d-flex d-column">
        <h2 class="text-white margin-right">DC</h2>
        <ul>
          <li v-for="(link, index) in links2" :key="index">
            <a :href="link.url" :class="{ active: link.active }">{{
              link.text
            }}</a>
          </li>
        </ul>
      </nav>
      <nav class="margin-top d-flex d-column">
        <h2 class="text-white margin-right">SITES</h2>
        <ul>
          <li v-for="(link, index) in links3" :key="index">
            <a :href="link.url" :class="{ active: link.active }">{{
              link.text
            }}</a>
          </li>
        </ul>
      </nav>
      <nav class="margin-top d-flex d-column">
        <h2 class="text-white margin-right">SHOP</h2>
        <ul>
          <li v-for="(link, index) in links4" :key="index">
            <a :href="link.url" :class="{ active: link.active }">{{
              link.text
            }}</a>
          </li>
        </ul>
      </nav>
    </section>
    <section>
      <figure class="p-relative">
        <img src="../assets/img/dc-logo-bg.png" alt="Logo dc" />
      </figure>
    </section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      links1: [
        { text: "Character", url: "#", active: false },
        { text: "Comics", url: "#", active: false },
        { text: "Movies", url: "#", active: false },
        { text: "Tv", url: "#", active: false },
        { text: "Games", url: "#", active: false },
        { text: "Videos", url: "#", active: false },
        { text: "News", url: "#", active: false },
      ],
      links2: [
        { text: "Terms Of Use", url: "#", active: false },
        { text: "Privacy policy (New)", url: "#", active: false },
        { text: "Ad Choices", url: "#", active: false },
        { text: "Advertising", url: "#", active: false },
        { text: "Jobs", url: "#", active: false },
        { text: "Subcriptions", url: "#", active: false },
        { text: "Talent Workshops", url: "#", active: false },
        { text: "CPSC Certificates", url: "#", active: false },
        { text: "Ratings", url: "#", active: false },
        { text: "Shop Help", url: "#", active: false },
        { text: "Contact Us", url: "#", active: false },
      ],
      links3: [
        { text: "Dc", url: "#", active: false },
        { text: "MAD Magazine", url: "#", active: false },
        { text: "DC Kids", url: "#", active: false },
        { text: "DC Universe", url: "#", active: false },
        { text: "Dc Power Visa", url: "#", active: false },
      ],
      links4: [
        { text: "Shop DC", url: "#", active: false },
        { text: "Shop DC Collectbles", url: "#", active: false },
      ],
    };
  },
};
</script>

<style scoped>
footer {
  height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
}

.d-flex {
  display: flex;
}

.f-wrap {
  flex-wrap: wrap;
}

.d-column {
  flex-direction: column;
}
footer section {
  width: 50%;
}

footer section nav {
  width: 33%;
}

ul {
  list-style-type: none;
  justify-content: center;
  align-items: center;
}

li a {
  text-decoration: none;
  padding: 10px 10px;
  color: white;
}

li a:hover,
li a.active {
  color: blue;
}

.text-white {
  color: white;
}

.margin-top {
  margin-top: 25px;
}

.margin-right {
  margin-left: 10px;
}

.p-relative {
  position: relative;
}

footer section figure img {
  position: absolute;
  transform: translate(30%, -20%);
}
</style>