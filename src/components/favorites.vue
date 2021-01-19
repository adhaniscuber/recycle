<template>
  <div id="favorites">
    <h3>Produk <span class="text-brand">Recycle</span> terfavorit!</h3>
    <div class="list-wrapper">
      <ProductItem v-for="(item, index) in products" :key="index" />
    </div>
  </div>
</template>

<script>
import ProductItem from "../components/product-item.vue";

export default {
  components: {
    ProductItem,
  },
  data: function () {
    return {
      products: [1, 2, 3, 4],
    };
  },
};
</script>

<style scoped>
h3 {
  text-align: left;
}
.list-wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-gap: 36px;
}
.text-brand {
  font-weight: 600;
  color: #81c784;
}
</style>
