<template>
  <main class="home">
    <div class="background-image">
      <img src="~/assets/images/background-img.jpg" />
    </div>
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
  margin: auto;
  display: grid;
  grid-template-columns: 1.6rem 1fr 1.6px;
  grid-template-rows: 4rem 1fr 4rem;
}
.home .background-image {
  grid-column: 1/-1;
  grid-row: 1/-1;
}
.home .masthead {
  grid-column: 2/4;
  grid-row: 1;
}
/* .home .app-subtitle {
  grid-column: 2/-2;
  grid-row: 2;
}
.home .app-description {
  grid-column: 2/-2;
  grid-row: 3;
} */
@media (min-width: 480px) {
  .home {
    grid-template-columns: 10rem 10rem 1fr 1fr 1fr 1fr 1fr;
    grid-template-rows: 10rem 5rem max-content max-content max-content;
  }
  .home .background-image {
    grid-column: 3/-1;
    grid-row: 1/-1;
  }
  .home .masthead {
    grid-column: 2/-1;
    grid-row: 3;
  }
}
</style>