<template>
  <section class="menu">
    <div class="user">
      <img
        src="../../static/logo.png"
        alt="网站logo图片"
      >
    </div>
    <ul class="menu-list">
      <li class="menu-item">
        <router-link
          to="/"
          exact
          class="no-underline"
        >首页</router-link>
      </li>
      <li class="menu-item">
        <router-link
          to="/postlist"
          exact
          class="no-underline"
        >文章列表</router-link>
      </li>
      <li class="menu-item">
        <router-link
          to="/edit"
          exact
          class="no-underline"
        >新增文章</router-link>
      </li>
      <li class="menu-item">
        <router-link
          to="/category"
          exact
          class="no-underline"
        >分类管理</router-link>
      </li>
      <li class="menu-item">
        <router-link
          to="/tag"
          exact
          class="no-underline"
        >标签管理</router-link>
      </li>
      <li class="menu-item">
        <router-link
          to="/laboratory"
          exact
          class="no-underline"
        >实验室</router-link>
      </li>
    </ul>
  </section>
</template>

<script>

export default {
  components: {},
  name: '',
  data() {
    return {

    }
  },
  methods: {

  },
  created() {

  },
  mounted() {

  },
}
</script>

<style scoped lang='less'>
@import "../assets/less/index";
.menu {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  width: 12em;
  background: #495060;
  z-index: 9999;

  .user {
    padding: 3em;

    img {
      width: 100%;
      height: 100%;
      transition: all 0.8s;
      &:hover {
        transform: scale(1.2) rotate(360deg);
      }
    }
  }
  .menu-list {
    text-align: center;

    .menu-item {
      display: block;
      width: 100%;
      font-size: 1.2em;
      line-height: 3;
    }
    a {
      color: hsla(0, 0%, 100%, 0.7);
      display: inline-block;
      width: 100%;
      &.router-link-exact-active {
        color: #fff;
        background: @base-color;
      }
    }
  }
}
</style>
