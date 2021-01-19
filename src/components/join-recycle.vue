<template>
  <div id="join">
    <img
      class="kv-banner"
      src="../assets/illustaration.svg"
      alt="illustration"
    />
    <div class="desc">
      <h3>
        Jadilah pahlawan Bumi!
        <span><img src="../assets/ion_earth.svg" alt="" /></span>
      </h3>
      <p>
        Dunia membutuhkanmu sekarang! Mari selamatkan Bumi dengan cara
        mendonasikan sampahmu yang masih layak pakai.
      </p>
      <button>Recycle</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Join",
};
</script>

<style scoped>
#join {
  width: 100%;
  display: flex;
  margin: 32px 0;
  align-items: center;
}
img.kv-banner {
  width: 390px;
}
h3 {
  text-align: left;
  font-size: 36px;
  vertical-align: middle;
  color: #81c784;
  margin: 8px 0;
}
h3 img {
  margin-bottom: -8px;
}
p {
  margin: 0;
  text-align: left;
  font-size: 18px;
  color: #c4c4c4;
}
button {
  width: 240px;
  height: 56px;
  border-radius: 8px;
  background-color: #81c784;
  outline: none;
  border: none;
  padding: 4px 24px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  font-size: 24px;
  font-weight: 600;
  margin: 16px 0;
}
div.desc {
  margin-left: 16px;
}
</style>
