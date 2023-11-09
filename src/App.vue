<script setup>
import contactInfo from "./components/contactInfo.vue";
import portfolioProjects from "./components/portfolioProjects.vue";
</script>

<template>
  <main class="wrapper">
    <div class="left-side">
      <contactInfo />
    </div>
    <div class="right-side">
      <portfolioProjects />
    </div>
  </main>
</template>

<style>
.wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

@media (min-width: 768px) {
  .wrapper {
    flex-direction: row;
  }
  .left-side {
    display: flex;
    height: 100vh;
    align-items: center;
    position: sticky;
    top: 0;
    margin-left: 2rem;
  }
  .right-side {
    margin-right: 2rem;
  }
}
</style>
