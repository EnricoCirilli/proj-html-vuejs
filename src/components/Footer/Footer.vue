<script>
// Import component Client section
import Client from "/src/components/Footer/Client.vue"
// Import component Info footer
import InfoFooter from "/src/components/Footer/InfoFooter.vue";

export default {
  name: "Footer",
  components: {
    Client,
    InfoFooter,
  },
  data() {
    return {
      //* Clients data array
      clients: [
        {
          img: ("src/assets/images/client-logos-3.png"),
          text: "TurboPower",
        },
        {
          img: ("src/assets/images/client-logos-1.png"),
          text: "Healthy",
        },
        {
          img: ("src/assets/images/client-logos-4.png"),
          text: "Color People",
        },
        {
          img: ("src/assets/images/client-logos-2.png"),
          text: "Health",
        },
      ],
      //* Departments data array
      departments: [
        "Cardiology",
        "Pediactrics",
        "Diabetes Care",
        "Ultrasound Echocardiogram",
      ],
    };
  },
};
</script>


<template>
  <footer>
    <Client :clients="clients" />
    <InfoFooter :departments="departments" />
    <section id="copyright">
      <div class="container copy-container">
        <i class="far fa-copyright"></i>
        <div class="text-copyright">
          Copyright - 2020 | Adava Theme by
          <span class="text-dark-grey">Theme Fusion</span>
          | All Rights Reserved | Powered by
          <span class="text-dark-grey">Wordpress</span>
        </div>
      </div>
    </section>
  </footer>
</template>



<style lang="scss" scoped>
// General style
</style>