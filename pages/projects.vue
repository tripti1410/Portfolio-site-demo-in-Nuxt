<template>
  <main class="projects-page">
    <section>
      <h1 class="title">Projects</h1>
      <div v-for="project in githubProjects" :key="project.id" class="project">
        <h3 class="project-title">
          <a :href="project.html_url">{{ project.name }}</a>
        </h3>
        <p class="stars">✷ {{ project.stargazers_count }}</p>
        <p>{{ project.homepage }}</p>
        <p>{{ project.description }}</p>
      </div>
    </section>
    <aside>
      <h3 class="aside-title">About</h3>
      <p class="aside-description">
        I create projects in github for experiments and fun. Not all projects are fully functional or pixel perfect.
        Few projects are the company's assignments and completed in time limits.
      </p>
      <p class="aside-description">
        I do experiment at
        <a href="https://codepen.io/tripti1410">Codepen</a>, mostly on CSS Grid layout, SVG's and Animations.
        You can find more about me at
        <a
          href="https://www.iamtrapti.com/"
        >website</a>
      </p>
    </aside>
  </main>
</template>

<script>
import { mapState } from "vuex";
export default {
  computed: { ...mapState(["githubProjects"]) }
};
</script>

<style>
.projects-page {
  max-width: 1200px;
  width: 100vw;
  margin: auto;
  display: grid;
  grid-template-areas: "projectSection" "asideAbout";
  grid-gap: 3.2rem;
}
.projects-page section {
  grid-area: projectSection;
  background-color: aliceblue;
  padding: 2.4rem 1.6rem 1.6rem 2.4rem;
}
.projects-page .project {
  margin-bottom: 1.6rem;
}
.projects-page .stars {
  color: orange;
}
.projects-page .title {
  margin-bottom: 1.6rem;
}
.projects-page aside {
  grid-area: asideAbout;
  padding: 0 1.6rem 2.4rem 2.4rem;
}
.projects-page .project-title {
  text-transform: capitalize;
}
.projects-page .aside-title {
  margin-bottom: 1.6rem;
}
.projects-page .aside-description {
  margin-bottom: 0.8rem;
}

@media (min-width: 480px) {
  .projects-page {
    grid-template-columns: 5fr 2fr;
    grid-template-areas: "projectSection asideAbout";
  }
  .projects-page aside {
    padding: 0;
  }
}
</style>