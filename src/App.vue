<template>
  <div>
    <mainheader />
    <ai />
    <newCarousel />
    <client />
    <cFooter />
  </div>
</template>

<script>
import mainheader from "./components/Header.vue";
import ai from "./components/AI.vue";
import newCarousel from "./components/carousel.vue";
import client from "./components/ClientsSay.vue";
import cFooter from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    mainheader,
    ai,
    newCarousel,
    client,
    cFooter,
  },
};
</script>

<style lang="scss">
// CSS IMPORTS
@import "./assets/scss/_colors.scss";
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;600;800&display=swap");
button {
  cursor: pointer;
  &:hover {
    opacity: 0.9;
  }
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
ul {
  list-style: none;
  li {
    margin-top: 0;
    a {
      text-decoration: none;
      &:hover {
        color: $base-color * 2;
      }
    }
  }
}
body {
  font-family: "Open Sans";
  color: #fff;
}
.base_btn {
  background: $base-color;
  padding: 15px 30px;
  border: none;
  border-radius: 7px;
  color: #fff;
}
</style>
