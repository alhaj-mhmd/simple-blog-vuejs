<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js Simple Blog App" />
    <img class="mali" alt="Vue logo" src="../assets/mali.jpg" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
};
</script>
<style lang="css">
.mali{
     width: 144px;
    height: 94px;
}
  
</style>
