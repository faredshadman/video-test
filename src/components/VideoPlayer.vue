<template>
  <div>
    <video controls>
      <source
        @play="play"
        src="http://173.212.238.58:8082/videos/atv-2022-01-30-07-01-04_BETA_CHAMPION_35-2022-01-30-07-40-47.mp4"
        type="video/mp4"
      />
    </video>
  </div>
</template>

<script>
export default {
  setup() {},
};
</script>

<style scoped>
div {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: red;
  height: 400px;
  width: 600px;
}
video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
