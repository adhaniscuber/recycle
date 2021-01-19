<template>
  <div class="category-item">
    <div class="image-wrapper centered">
      <img :src="require(`../assets/${category.icon}.svg`)" alt="" />
    </div>
    <div>
      <p>{{ category.name }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    category: Object,
  },
  computed: {
    setIcon() {
      return `../assets/${this.category.icon}.svg`;
    },
  },
};
</script>

<style scoped>
.centered {
  display: flex;
  justify-content: center;
  align-self: center;
}
div.image-wrapper {
  height: 80px;
  width: 100%;
}
.category-item {
  border: 1px solid #e5e5e5;
  border-radius: 8px;
  min-height: 120px;
}
</style>
