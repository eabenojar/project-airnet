<template>
  <div class="navbar">
    <nuxt-link class="home" to="/">Home</nuxt-link>
    <ul class="main-nav">
      <li v-for="(item, index) in items" :key="index">
        <nuxt-link :to="item.link">{{item.title}}</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: "Interviews",
          link: "/interviews"
        },
        {
          title: "Positions",
          link: "/positions"
        },
        {
          title: "Projects",
          link: "/projects"
        },
        {
          title: "Take Home ",
          link: "/takehometests"
        }
      ]
    };
  }
};
</script>

<style scoped>
.navbar {
  height: 3rem;
  width: 100vw;
  display: flex;
  justify-content: space-between;
  padding-bottom: 0;
  align-items: center;
}
.home {
  text-decoration: none;
  color: #000;
  display: inline-block;
  font-size: 12px;
  margin-top: 10px;
  margin-left: 20px;
}
.main-nav {
  display: flex;
  justify-content: flex-end;
  margin-right: 30px;
  flex-direction: row;
}
.navbar ul {
  list-style-type: none;
}
.navbar ul li a {
  text-decoration: none !important;
  color: #333333;
  margin-left: 30px;
  font-size: 0.75rem;
}
</style>
