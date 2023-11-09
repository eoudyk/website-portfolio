<script setup>
import Card from "./pageCard.vue";
import carouselPlanharbour from "./carouselPlanharbour.vue";
import carouselBrainflix from "./carouselBrainflix.vue";
</script>
<template>
  <div class="projects-container">
    <h1 class="projects__title">Projects</h1>
    <Card>
      <template v-slot:title>
        <h2 class="project__title">Planharbour</h2>
      </template>
      <template v-slot:content>
        <carouselPlanharbour />
        <ul class="project__stack">
          <ol class="project__stack-item">
            Axios
          </ol>
          <ol class="project__stack-item">
            mySQL
          </ol>
          <ol class="project__stack-item">
            Sass
          </ol>
          <ol class="project__stack-item">
            Express
          </ol>
          <ol class="project__stack-item">
            Vite
          </ol>
          <ol class="project__stack-item">
            Node.js
          </ol>
          <ol class="project__stack-item">
            API: ChatGPT
          </ol>
          <ol class="project__stack-item">
            knex.js
          </ol>
        </ul>
        <p class="project__description">
          This was capstone project for my Software Engineer bootcamp at
          BrainStation. This project was put together in under 2 weeks (while
          sick with COVID) but provides a solution to a problem I used to
          regularly incur when I worked as a teacher. When teachers need to be
          away for illness or appointments, they are expected to create highly
          detailed plans for their supply teacher to use. Planharbour will
          create supply plans in minutes (as opposed to hours) using chatGPT and
          form validation.
        </p>
      </template>
    </Card>

    <Card>
      <template v-slot:title>
        <h2 class="project__title">Brainflix</h2>
      </template>
      <template v-slot:content>
        <carouselBrainflix />
        <ul class="project__stack">
          <ol class="project__stack-item">
            Axios
          </ol>
          <ol class="project__stack-item">
            Sass
          </ol>
          <ol class="project__stack-item">
            Express
          </ol>
          <ol class="project__stack-item">
            React
          </ol>
          <ol class="project__stack-item">
            uuid
          </ol>
        </ul>
        <p class="project__description">
          A mock SPA site for streaming videos. This project was completed in
          three sprints (1 week each). Styling was provided in mock-ups and
          followed responsive design specifications. At this time, the Github
          link is unavailable as the project is part of BrainStation's
          intellectual property.
        </p>
      </template>
    </Card>

    <Card>
      <template v-slot:title>
        <h2 class="project__title">Scotiabank-hackathon</h2>
      </template>
      <template v-slot:content>
        <div class="project__video">
          <video controls width="250">
            <source
              src="../assets/screenshots/scotia/scotia-mobile.mp4"
              type="video/mp4"
            />
          </video>
        </div>
        <ul class="project__stack">
          <ol class="project__stack-item">
            React
          </ol>
          <ol class="project__stack-item">
            Sass
          </ol>
        </ul>
        <p class="project__description">
          A 24 hour industry sponsored hackathon project. Working
          cross-collaboratively with UX designers as well as Data Scientists,
          this is the front end to my team's "modeled" mobile-first solution to
          the sponsored problem: connecting clients to specialized financial
          advisors.
        </p>
      </template>
    </Card>
  </div>
</template>

<script>
export default {
  name: "portfolioProjects",
};
</script>

<style scoped>
ul {
  margin: 0;
  padding: 0;
}
.projects-container {
  margin-top: 1rem;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.projects__title {
  background: #fcc140;
  padding: 0.25rem 0.5rem;
}
.project__title {
  font-weight: bold;
  margin: 1rem;
  display: flex;
  justify-content: center;
}
.project__img {
  width: 100%;
}
.project__video {
  display: flex;
  justify-content: center;
}

.project__stack {
  display: flex;
  flex-wrap: wrap;
}

.project__stack-item {
  background: #fcc140;
  padding: 0.25rem 0.5rem;
  margin: 0.5rem 0.25rem;
}

@media (min-width: 768px) {
  .projects-container {
    margin: 2rem;
  }
}
</style>
