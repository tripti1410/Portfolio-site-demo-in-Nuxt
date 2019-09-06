<template>
  <main class="home">
    <!-- <div class="background-image">
      <img src="~/assets/images/background-img.jpg" />
    </div>-->
    <header class="masthead">
      <h1 class="app-title">Hello, I'm Trapti Rahangdale</h1>
      <h2 class="app-subtitle">Frontend Developer</h2>
      <p
        class="app-description"
      >Interested in building responsive, interactive, performant and accessible web apps.</p>
    </header>
  </main>
</template>

<script>
export default {};
</script>

<style>
.home {
  max-width: 1200px;
  width: 100%;
  min-height: 35rem;
  margin: auto;
  display: grid;
  grid-template-columns: 1.6rem 1fr 1.6px;
  grid-template-rows: 4rem 1fr 4rem;
  background: url("~assets/images/background-img.jpg") no-repeat center center;
  background-size: 100% 100%;
  background-blend-mode: multiply;
  background-color: aliceblue;
}

.home .masthead {
  grid-column: 2/4;
  grid-row: 1;
  mix-blend-mode: color-burn;
}
@media (min-width: 480px) {
  .home {
    min-height: 70rem;
    grid-template-columns: 15rem 1fr 1fr 1fr 1fr 5rem;
    grid-template-rows: 5rem max-content max-content max-content;
  }
  .home .masthead {
    grid-column: 4/7;
    grid-row: 3;
  }
}
</style>