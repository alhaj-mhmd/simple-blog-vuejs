<template>
  <div class="about">
    <h1>{{ pageName }}</h1>
    <a :href="pageDescription">{{ pageDescription }}</a>
    <div>
</div>
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      pageName: "About Us",
      pageDescription: "https://www.linkedin.com/in/mohammad-alhaj-ali/"};

  },
  name: "about",
};
</script>
