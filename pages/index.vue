<template>
  <main class="home">
    <header class="masthead">
      <h1 class="app-title">Hello, I'm Trapti Rahangdale</h1>
      <h2 class="app-subtitle">Frontend Developer</h2>
      <p
        class="app-description"
      >Interested in building responsive, interactive, performant and accessible web apps.</p>
    </header>
    <p class="photo-credit">
      Photo by
      <a
        class="link"
        href="https://unsplash.com/@johnmarkarnold?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText"
        target="_blank"
      >John Mark Arnold</a> on
      <a class="link" href="https://unsplash.com" target="_blank">Unsplash</a>
    </p>
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
  background-size: cover;
  background-blend-mode: multiply;
  background-color: aliceblue;
}

.home .masthead {
  grid-column: 2/4;
  grid-row: 1;
  mix-blend-mode: color-burn;
}
.photo-credit {
  grid-column: span 3 /-1;
  grid-row: span 1 / -1;
  align-self: center;
  justify-self: end;
  padding-right: 0.8rem;
}
@media (min-width: 480px) {
  .home {
    min-height: 70rem;
    grid-template-columns: 15rem 1fr 1fr 1fr 1fr 5rem;
    grid-template-rows: 5rem max-content max-content max-content 1fr 1fr 0.5fr;
  }
  .home .masthead {
    grid-column: 4/7;
    grid-row: 3;
  }
}
</style>