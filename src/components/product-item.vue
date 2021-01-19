<template>
  <div class="product">
    <img v-if="false" src="null" />
    <div v-else class="product-img" />
    <div class="product-bio">
      <p class="text text-dist">{{ item.distributor }}</p>
      <p class="text text-title product-name">{{ item.name }}</p>
      <p class="text text-title">
        <span class="text text-price">Rp. {{ item.price }}</span
        >/{{ item.unit }}
      </p>
      <p class="text text-caption">min. {{ item.minimal }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      item: {
        distributor: "re:earth distribution",
        name: "Kertas HVS 60gr",
        price: 2000,
        unit: "kg",
        minimal: "10kg",
      },
    };
  },
};
</script>

<style scoped>
.product-img {
  background-color: rgba(129, 199, 132, 15%);
  border-radius: 8px;
  width: 200px;
  height: 200px;
  border: none;
  display: inline-block;
}
.product-bio {
  padding: 0 8px;
}
.text {
  margin: 0;
  color: #35394c;
  text-align: left;
}
.text-dist {
  color: #81c784;
  font-size: 11px;
  font-weight: 100;
  margin-bottom: 4px;
}
.text-title {
  font-size: 14px;
}
.product-name {
  margin-bottom: 16px;
}
.text-price {
  font-weight: 600;
}
.text-caption {
  font-size: 11px;
}
</style>
