<template>
  <div>
    <app-nav />
    <nuxt />
  </div>
</template>
<script>
import AppNav from "~/components/AppNav.vue";
export default {
  components: {
    AppNav
  }
};
</script>
<style>
html {
  font-family: "Roboto", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  font-size: 62.5%;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
body {
  font-size: 1.8rem;
}
h1,
h2,
h3 {
  font-family: "Alfa Slab One", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-weight: normal;
  letter-spacing: 1px;
}

h1 {
  font-size: 3.6rem;
}

h2 {
  font-size: 3rem;
}

img {
  max-width: 100%;
}

a,
a:visited,
a:active {
  color: inherit;
  text-decoration: none;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
