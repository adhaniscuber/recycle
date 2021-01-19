<template>
  <div id="home">
    <Navbar />
    <div class="container">
      <Categories />
      <Favorites />
      <Join />
    </div>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/navbar.vue";
import Categories from "../components/categories.vue";
import Join from "@/components/join-recycle.vue";
import Favorites from "../components/favorites.vue";
import Footer from "../components/footer.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    Categories,
    Join,
    Favorites,
    Footer,
  },
};
</script>

<style scoped>
#home {
  margin-top: 80px;
  padding: 16px 0;
}
.container {
  max-width: 912px;
  margin: 0 auto;
}
</style>
