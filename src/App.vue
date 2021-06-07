<template>
  <Header />
  <router-view />
  <Footer />
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
  },
};
</script>

<style lang="scss">
//fonts
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@600&family=Paprika&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap");

$paprika: "Paprika", cursive;
$os: "Open Sans", sans-serif;
$montserrat: "Montserrat", sans-serif;
//colors
:root {
  --paprika: "Paprika", cursive;
  --montserrat: "Montserrat", sans-serif;
  --main: #440d3d;
  --lt-main: #e63462;
  --op-main: #fbfbfb;
}
*,
*:before,
*:after {
  box-sizing: inherit;
  text-decoration: none;
  list-style-type: none;
  margin: 0;
  padding: 0;
  color: var(--main);
  -webkit-tap-highlight-color: transparent;
}

body {
  box-sizing: border-box;
  font-family: $montserrat;
  font-weight: 600;
  line-height: 1.4;
  font-size: 16px;
  display: flex;
  flex-direction: column;
  background: var(--op-main);
  overflow-x: hidden;
}
button {
  background: none;
  border: none;
  font-family: $montserrat;
  font-weight: 600;
  line-height: 1.4;
  font-size: 16px;
}
</style>
