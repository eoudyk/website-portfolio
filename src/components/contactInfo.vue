<script setup>
import Headshot from "../components/icons/IconHeadshot.vue";
import Learning from "../components/icons/learningIcon.vue";
import Dog from "../components/icons/dog-puppy-face-icon.vue";
</script>

<template>
  <div class="contact-container">
    <div class="bubble">
      <Headshot />
      <svg
        class="bubble__tiny"
        width="20"
        height="20"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="10" cy="10" r="10" fill="#fcc140" />
      </svg>
      <Dog />
      <svg
        class="bubble__medium"
        width="50"
        height="50"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="25" cy="25" r="25" fill="#fcc140" />
      </svg>
      <Learning />
      <svg
        class="bubble__tiny"
        width="20"
        height="20"
        xmlns="http://www.w3.org/2000/svg"
      >
        <circle cx="10" cy="10" r="10" fill="#fcc140" />
      </svg>
    </div>
    <div class="contact__details">
      <h1 class="name">Emily Oudyk</h1>
      <div class="links">
        <a
          href="https://www.linkedin.com/in/emilyoudyk/"
          class="linkedIn"
          target="_blank"
          >LinkedIn</a
        >
        <a href="https://github.com/eoudyk" class="github" target="_blank"
          >Github</a
        >
      </div>
      <div class="contact-about">
        Hi there and welcome to my site! I am a passionate Software Engineer
        with a background in education and Program Coordination.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "contactInfo",
};
</script>

<style scoped>
.contact-container {
  padding-bottom: 2rem;
  border-bottom: 1px solid #fcc140;
}
.bubble {
  display: flex;
  margin-top: 4rem;
}
.bubble__tiny {
  margin-top: -2rem;
}
.bubble__medium {
  margin: 1rem;
  margin-top: -1rem;
}

.linkedIn {
  margin-right: 1rem;
  padding: 0.25rem;
  background: #fcc140;
}

.github {
  padding: 0.25rem;
  background: #fcc140;
}

.contact-about {
  margin-top: 1.5rem;
}
@media (min-width: 768px) {
  .contact-container {
    border-bottom: none;
    border-right: 1px solid #fcc140;
    padding-right: 2rem;
    margin-left: 1rem;
  }
}
</style>
