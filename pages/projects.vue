<template>
  <main class="codepens-page">
    <section>
      <h1>Projects</h1>
      <div v-for="project in githubProjects" :key="project.id" class="project">
        <h3>
          <a :href="project.html_url">{{ project.name }}</a>
        </h3>
        <p class="stars">✷ {{ project.stargazers_count }}</p>
        <p>{{ project.homepage }}</p>
        <p>{{ project.description }}</p>
      </div>
    </section>
    <aside></aside>
  </main>
</template>

<script>
import { mapState } from "vuex";
export default {
  computed: { ...mapState(["githubProjects"]) }
};
</script>

<style>
.codepens-page {
  max-width: 1200px;
  width: 100%;
  margin: auto;
  display: grid;
  grid-template-columns: 5fr 2fr;
}
.codepens-page section {
  background-color: white;
  color: black;
  padding: 3rem;
}
</style>