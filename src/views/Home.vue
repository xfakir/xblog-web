<template>
  <div class="home">
    <navbar>navbar</navbar>
    <profile>profile</profile>
    <main-content>main-content</main-content>
    <toolbar>toolbar</toolbar>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {
    Navbar: () => import("@/views/Navbar"),
    Profile: () => import("@/views/Profile"),
    MainContent: () => import("@/views/MainContent"),
    Toolbar: () => import("@/views/Toolbar")
  }
};
</script>

<style scoped>
.home {
  height: 100vh;
  background: url("../assets/backgroud.jpg") no-repeat center;
  background-size: 100%;
}
</style>
