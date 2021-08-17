<template>
  <div class="card-container">
    <img
      :src="require(`@/assets/images/${card.image || fe7.jpg}`)"
      alt=""
      class="image"
    />
  </div>
</template>

<script>
export default {
  props: ["card"]
};
</script>

<style scoped>
.card-container {
  border-radius: 0.5rem;
  cursor: pointer;
  height: 12.5rem;
  margin-bottom: 1.5rem;
  overflow: hidden;
  width: 24%;
}
.image {
  width: 100%;
  height: 100%;
}
</style>
