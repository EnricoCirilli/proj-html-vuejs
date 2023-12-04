<script>
export default {
  name: "NavItems",
  props: ["nav"],
};
</script>
  
<template>  
  <!-- NAVIGATION BAR -->
  <div id="nav-bar">
    <ul>
      <!-- V-for to cycle in the data array of the nav-bar -->
      <li v-for="item in nav" :key="item.id">
        <a :href="item.url" :class="{ active: item.current }" class="uppercase">
          {{ item.text }}
        </a>
      </li>
    </ul>
    <!-- Navigation bar button  -->
    <button class="uppercase clickable btn-primary-color">
      make appointment
    </button>
  </div>

</template>
  
  <style lang="scss" scoped>

  //// NAV-BAR STYLE
#nav-bar {
  display: flex;
  align-items: center;
  font-size: 10px;
  font-weight: lighter;
}
//* Style nav-bar item 
ul {
  display: flex;
  li {
    list-style-type: none;
    a {
      text-decoration: none;
      color: white;
      padding: 0 20px;
        &.active, &:hover  
      {
         color:  #39afbb; ;
       }
    }
  }
}
//* Button nav-bar style
button {
  font-size: 10px;
  font-weight: lighter;
  padding: 6px 16px;
}
</style>