<template>
  <div>
    <h1>xezer : BETA_CHAMPION_35 (27-05-2022 11:46:20)</h1>
    <video controls>
      <source
        @play="play"
        :src="require('@/assets/video.mp4')"
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
  background: black;
  height: 400px;
  width: 600px;
}
video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
