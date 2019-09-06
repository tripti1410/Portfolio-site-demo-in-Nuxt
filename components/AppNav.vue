<template>
  <nav class="app-navigation">
    <ul>
      <li>
        <nuxt-link exact to="/">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/projects">Projects</nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {};
</script>

<style>
.app-navigation {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100px;
}
.app-navigation ul {
  padding: 0 0;
  margin: 0;
}
.app-navigation ul li {
  display: inline-block;
  padding: 1.6rem;
  font-size: 2.4rem;
  font-weight: 500;
}
</style>