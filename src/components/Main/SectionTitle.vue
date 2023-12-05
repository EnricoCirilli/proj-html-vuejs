<script>
export default {
  name: "WelcomeTitle",
  props: ["welcomeInfo"],
};


</script>

<template>
  <section id="welcome-title" class="container">
    <h1>Avada Health</h1>
    <h2>Medical Solutions for Your Health</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum explicabo
      in vitae iste placeat adipisci iusto provident laudantium nisi. Et.
    </p>
    <div class="welcome-info">
      <WelcomeCard v-for="info in welcomeInfo" :key="info.id" :info="info" />
    </div>
  </section>
</template>


<style>


</style>

