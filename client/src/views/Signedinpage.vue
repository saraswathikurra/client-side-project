<template>
  <div class="signedinpage">
    <h1>Select an Exercise </h1>
    <br>
    <p>You can track your daily activities using this Website.</p>
    <p>We also provide with the food plans. Check our Food section for a meal plan.</p>
    <img src='./../assets/background.png'  v-on:click="swim_video" alt="exercise1" width="300" height="200" border = "5">
    <img src='./../assets/background.png' alt="exercise1" width="300" height="200">
    <img src='./../assets/background.png' alt="exercise1" width="300" height="200">
    <img src='./../assets/background.png' alt="exercise1" width="300" height="200">
    <div id="video_player">
      <video ref="videoRef" src="" width="50%" id="video-container"  controls></video>
    </div>

   </div>
</template>
<script>
export default{
  el: "#video_player",
  methods: {
    swim_video() {
      console.log("got to swim for sure")
    this.$refs.videoRef.src = "./../media/swim.mp4";
    this.$refs.videoRef.play();
  }
}
}

</script>