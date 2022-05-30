<template>
  <button @click="handleVideo">Show video modal</button>
  <VideoPlayer v-show="video" />
</template>

<script>
import { ref } from "@vue/reactivity";
import VideoPlayer from "./components/VideoPlayer.vue";

export default {
  name: "App",
  components: {
    VideoPlayer,
  },
  setup() {
    const video = ref(false);
    const handleVideo = () => {
      video.value = !video.value;
      console.log(video);
    };

    return {
      video,
      handleVideo,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
