<script>
// Nav component import
import NavItems from "./NavItems.vue";

export default {
  name: "Header",
  components: {
    NavItems,
  },
  data() {
    return {
      // Barra di navigazione e data array
      nav: [
        {
          id: "1",
          text: "home",
           url: "#",
           current: true,
        },
        {
           id: "2",
          text: "about",
           url: "#",
           current: false,
        },
        {
          id: "3",
          text: "departments",
          url: "#",
          current: false,
        },
        {
          id: "4",
          text: "articles",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <header class="bg-header">
    <!-- HEADER TOP -->
     <section id="header-bar" class="container"> 
      <!-- Logo  -->
      <a href="#">
        <img
          id="logo"
          src="./assets/images/medical_logo_1x_light.png"
          alt="logo"
        />
      </a>
      <!-- Navigation bar  -->
      <nav>
        <NavItems :nav="nav" />
      </nav> 
    </section>
    <!-- HEADER BOTTOM -->
    <section id="spotlight" class="container-small">
      <div class="text-spotlight">
        <h2>
          <span>Caring </span>
          <span class="text-primary-color">For Life</span>
        </h2>
        <p>
          Kind words can be short and easy to speak, but their echoes are truly
          endless. Adava Health focuses on you as if it was our own family.
        </p>
        <button class="btn-spotlight uppercase btn-primary-color clickable">
          learn more
        </button>
      </div> 
    </section>
  </header>
</template>

<style lang="scss" scoped>

// LOGO
#logo {
  height: 30px;
}
// GENERAL HEADER STYLE

// Background header
.bg-header {
  background-image: url("src/assets/images/header-image-homepage.jpg");
  height: 74vh;
  background-size: cover;
}
//* Header bar style
#header-bar {
  height: 10vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.text-spotlight {
  width: 500px;
  margin-top: 100px;
  h2 {
  font-weight: lighter;
  font-size: 40px;
  color: white;
  margin-bottom: 15px;
  .text-primary-color {
    color: #39afbb;
  }
}
p {
  color: white;
  font-weight: 300;
  margin-bottom: 20px;
}
//* Spotlight button style 
.btn-spotlight {
  font-size: 12px;
  font-weight: lighter;
  padding: 6px 20px;
}
}
</style>
