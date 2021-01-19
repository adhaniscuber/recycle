<template>
  <div id="footer">
    <div class="us">
      <img src="../assets/logo.svg" />
      <p class="text-us">
        <span class="bold">Recycle </span>
        <span class="green">(re·cy·cle or rēˈsīk(ə)l)</span> is the process of
        converting waste materials into new materials and objects. The recovery
        of energy from waste materials is often included in this concept. The
        recyclability of a material depends on its ability to reacquire the
        properties it had in its virgin or original state.
      </p>
    </div>
    <div class="link-wrapper">
      <a class="link" href="#">About us</a>
      <a class="link" href="#">Contact</a>
      <a class="link" href="#">Blog</a>
    </div>
    <div style="display: flex">
      <img class="socmed" src="../assets/bx_bxl-instagram-alt.svg" alt="ig" />
      <img class="socmed" src="../assets/bx_bxl-youtube.svg" alt="yt" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#footer {
  padding: 32px 0;
  border-top: 1px solid #e4e4e4;
  display: flex;
  margin: 0 128px;
}
.us {
  display: flex;
  align-items: center;
}
.text-us {
  text-align: left;
  margin: 0 16px;
}
.bold {
  font-weight: 600;
}
.green {
  color: #81c784;
}
.link-wrapper {
  min-width: 120px;
  display: flex;
  flex-direction: column;
  margin-left: 32px;
}
.link {
  text-align: left;
  padding: 8px 0;
  color: #81c784;
  text-decoration: none;
}
.socmed {
  padding: 16px;
}
</style>
