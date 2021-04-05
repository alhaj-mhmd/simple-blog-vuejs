<template>
  <div class="post-box mt-3">
    <span class="post-views">{{ views }}</span>
    <h3 class="post-title">{{ title }}</h3>
    <span class="post-date">{{ date }}</span>
    <p class="post-content">{{ content }}</p>
    <div class="row">
      <div class="col-6">
        <span class="post-auther">{{ auther }}</span>
      </div>
      <div class="col-6 text-right">
        <span class="post-category">{{ category }}</span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["views", "title", "auther", "category", "content", "date"],
  name: "post",
};
</script>
<style lang="scss" scoped>
.post-box {
  padding: 15px;
  background-color: #fff;
  box-shadow: 0 0 10px #ddd;
  text-align: left;
  border-radius: 5px;
  position: relative;
  .post-views {
    position: absolute;
    top: 5px;
    right: 5px;
    background-color: #f9c4c4;
    padding: 1px 4px;
    border-radius: 4px;
    font-weight: bold;
    text-align: center;
  }
  .post-title {
    font-weight: bold;
    color: blue;
  }
  .post-date {
    display: block;
    padding: 0 0 5px;
    color: #888;
    font-size: 14px;
  }
  .post-content {
    color: #666;
    line-height: 1.8;
  }
  .post-auther {
    background-color: green;
    padding: 5px;
    color: #fff;
    border-radius: 5px;
  }
  .post-category {
    background-color: green;
    padding: 5px;
    color: #fff;
    border-radius: 5px;
  }
}
</style>
