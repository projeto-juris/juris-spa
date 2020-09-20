<template>
  <div>
    <v-app id="app">
      <v-main>
        <router-view />
      </v-main>
    </v-app>
  </div>
</template>
<script>
export default {};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap");
#app {
  font-family: "Poppins", sans-serif;
  background-image: url("assets/Background.png");
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
  overflow: hidden;
}
</style>
