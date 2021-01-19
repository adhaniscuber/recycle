<template>
  <nav id="navbar">
    <div class="container">
      <img src="../assets/logo-recycle.svg" alt="logo" />
      <div class="search-wrapper">
        <div class="location">
          <img src="../assets/jam_map-marker-f.svg" />
          <p>Jabodetabek</p>
        </div>
        <input type="text" placeholder="Cari apa aja ada..." />
      </div>
      <div class="right-menu">
        <img class="img-bell" src="../assets/bell.svg" alt="notification" />
        <button>
          <img src="../assets/1.svg" alt="notification" />
          Cart
        </button>
      </div>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
#navbar {
  box-shadow: 4px 4px 16px 0 rgba(128, 128, 128, 25%);
  height: 80px;
  position: fixed;
  width: 100%;
  background-color: #fff;
  top: 0;
  left: 0;
}
.container {
  height: inherit;
  margin: 0 128px;
  padding: 20px 0;
  display: flex;
  justify-content: space-around;
  align-items: center;
  box-sizing: border-box;
}
.search-wrapper {
  width: 100%;
  margin: 0px 16px;
  border: 1px solid #e5e5e5;
  border-radius: 8px;
  height: 40px;
  display: flex;
}
input {
  width: 100%;
  outline: none;
  border: none;
  padding: 0 16px;
  border-radius: 8px;
}
.right-menu {
  display: flex;
  align-items: center;
}
.img-bell {
  margin: 0 16px;
}

button {
  border-radius: 8px;
  background-color: #81c784;
  height: 40px;
  outline: none;
  border: none;
  padding: 4px 24px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
}

button img {
  margin-right: 12px;
}
.location {
  width: 200px;
  height: 38px;
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  background-color: #f2f2f2;
  border-right: 1px solid #e5e5e5;
}
.location p {
  margin: 0 8px;
}
.location img {
  margin-left: 16px;
}
</style>
