<template>
  <div id="app">
    <Header />
    <Shop />
    <Footer />
  </div>
</template>
<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Merriweather:wght@300;400;700&display=swap");

* {
  margin: 0;
  padding: 0;
  text-decoration: none;
  background-color: #f6f3f3;
  box-sizing: border-box;
  font-family: "Merriweather", serif;
}
</style>

<script>
import Header from "./components/header";
import Shop from "./components/shop";
import Footer from "./components/footer";

export default {
  name: "App",
  components: {
    Header,
    Shop,
    Footer,
  },
};
</script>


