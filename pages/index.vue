<template>
  <main class="home">
    <div class="background-image">
      <img src="~/assets/images/background-img.jpg" />
    </div>
    <h1 class="app-title">Hello, I'm Trapti Rahangdale</h1>
    <h2 class="app-subtitle">Frontend Developer</h2>
    <p
      class="app-description"
    >Interested in building responsive, interactive, performant and accessible web apps.</p>
  </main>
</template>

<script>
export default {};
</script>

<style>
.home {
  max-width: 1200px;
  width: 100%;
  margin: auto;
  display: grid;
  grid-template-columns: 200px 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 100px 100px 1fr 1fr 1fr;
}
.home .background-image {
  grid-column: 2/-1;
}
.home .app-title,
.home .app-subtitle,
.home .app-description {
  grid-column: 1/5;
}
.home .app-title {
  grid-row: 3;
}
.home .app-subtitle {
  grid-row: 4;
}
.home .app-description {
  grid-row: 5;
}
</style>