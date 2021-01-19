<template>
  <div class="categories-wrapper">
    <CategoryItem
      v-for="(item, index) in allCategory"
      :key="index"
      :category="item"
    />
    <CategoryItem :category="more" />
  </div>
</template>

<script>
import CategoryItem from "./category-item.vue";

const dataCategory = [
  {
    name: "Botol kaca",
    icon: "jam_bottle",
  },
  {
    name: "Botol plastik",
    icon: "jam_bottle",
  },
  {
    name: "Plastik",
    icon: "tabler_recycle",
  },
  {
    name: "Plastik keras",
    icon: "tabler_recycle",
  },
  {
    name: "Kertas",
    icon: "ph_newspaper-clipping",
  },
  {
    name: "Box kardus",
    icon: "bi_box-seam",
  },
  {
    name: "Box karton",
    icon: "bi_box-seam",
  },
];

export default {
  name: "categories",
  components: {
    CategoryItem,
  },
  data: function () {
    return {
      allCategory: dataCategory,
      more: {
        name: "Lainnya",
        icon: "gg_menu-grid-o",
      },
    };
  },
};
</script>

<style scoped>
.categories-wrapper {
  margin: 70px 0 48px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
  grid-gap: 16px;
}
</style>
