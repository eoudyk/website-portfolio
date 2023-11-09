<template>
  <div class="card">
    <slot name="title"></slot>
    <slot name="content"></slot>
  </div>
</template>
<script>
export default {
  name: "page-card",
};
</script>

<style scoped>
.card {
  box-shadow: 1px 1px 5px rgb(50, 50, 50);
  border-radius: 4px;
  padding: 1rem;
  margin: 1rem 0.5rem;
}
</style>
