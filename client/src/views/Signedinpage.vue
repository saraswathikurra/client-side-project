<template>
  <div class="signedinpage">
    <h1>Select an Exercise to View Description </h1>
    <br>
    <img src='./../assets/swim.jpg'  v-on:click="swim_video" alt="exercise1" width="300" height="200" border = "5">
    <img src='./../assets/yoga.jpg' v-on:click="yoga_exercise" alt="exercise1" width="300" height="200" border = "5">
    <img src='./../assets/zumba.jpg' v-on:click="zumba_exercise" alt="exercise1" width="300" height="200" border = "5">
    <img src='./../assets/background.png' v-on:click="gym_exercise" alt="exercise1" width="300" height="200" border = "5">
    <br>
     <br>
    <div >
     <h3 id="text_displayer"></h3>
    </div>

   </div>
</template>
<script>
export default{
  methods: {
    swim_video() {
      document.getElementById("text_displayer").textContent = "Swimmers at the beginner level may swim two to three times per week. If you are a beginner, then swim for alternative days. If you are a professional, then you can swim for 1 hour every day."; 
  },
  yoga_exercise() {
      document.getElementById("text_displayer").textContent = "Yoga is amazing—even if you only practice for one hour a week, you will experience the benefits of the practice. If you can do more than that, you will certainly experience more benefits. We suggest starting with two or three times a week, for an hour or an hour and a half each time. "; 
  },
  zumba_exercise() {
      document.getElementById("text_displayer").textContent = "How often you'll need to participate in Zumba to lose weight depends on your health and fitness goals. Aim to burn 300 to 400 calories per workout session, a minimum of three days a week. We suggest you to do Zumba on alternative days."; 
  },
  gym_exercise() {
      document.getElementById("text_displayer").textContent = "To lose weight, most adults need 60 to 90 minutes of moderately intense physical activity per day while keeping caloric intake in check. This can vary according to your diet, your age, weight, and gender, plus the types of workouts you do. If you are a beginner, then start with cardio for 2 weeks.If you are a professional, then work out for 2 hours every day."; 
  },

}
}

</script>