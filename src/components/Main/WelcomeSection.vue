<script>
// Import component title section
import SectionTitle from "./SectionTitle.vue";

// Import component card
import SectionCard from "./SectionTitle.vue";

export default {
  name: "WelcomeMain",
  components: {
    SectionTitle,
    SectionCard,
  },
data() {
    return {
      // Welcome info data array
      welcomeInfo: [
        {
          icon: "src/assets/images/icon-1.png",
          url: "#",
          title: "same day appointments",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
        {
          icon: "src/assets/images/icon-2.png",
          url: "#",
          title: "world class facilities",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
        {
          icon: "src/assets/images/icon-3.png",
          url: "#",
          title: "expert doctors",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
        {
          icon: "src/assets/images/icon-4.png",
          url: "#",
          title: "complementary therapies",
          text: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium",
        },
      ],
    };
  },
};
</script>


<template>



</template>



<style lang="scss" scoped>

#welcome-section {
  margin-bottom: 30px;
}
//? Hover effects
.card-info li:hover a h4 {
  color: #3aafbf;
}
.card-info li:hover a p {
  color: #46525f;
}

</style>