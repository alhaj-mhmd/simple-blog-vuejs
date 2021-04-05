<template>
  <div class="blog">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class="posts-area">
            <BlogPosts
              v-for="post in posts"
              :key="post.id"
              :views="post.views"
              :title="post.title"
              :date="post.date"
              :content="post.content"
              :auther="post.auther"
              :category="post.category"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import BlogPosts from "@/components/Blog/BlogPosts.vue";
import JsonPosts from "../json/blog_posts.json";

export default {
  data: function () {
    return {
      pageName: "Blog",
      pageDescription: "This is blog page",
      posts: JsonPosts,
    };
  },
  name: "blog",
  components: {
    BlogPosts,
  },
};
</script>
