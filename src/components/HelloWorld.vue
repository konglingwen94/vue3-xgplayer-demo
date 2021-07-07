<template>
  <div id="vs">xgplayer</div>
</template>

<script setup>
import { onMounted } from "vue";
import Player from "xgplayer";

onMounted(() => {
  const player = new Player({
    id: "vs",
    autoplay: false,
    playbackRate: [0.5, 0.75, 1, 1.5, 2],
    defaultPlaybackRate: 1.5,
    volume: 0.3,
    url: "//sf1-cdn-tos.huoshanstatic.com/obj/media-fe/xgplayer_doc_video/mp4/xgplayer-demo-720p.mp4",
    poster: "//lf9-cdn-tos.bytecdntp.com/cdn/expire-1-M/byted-player-videos/1.0.0/poster.jpg",
    playsinline: true,
    height: 399,
    // width: window.innerWidth
  });
});
</script>

<style scoped>
 
</style>
