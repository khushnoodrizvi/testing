<template>
  <header class="header">
    <div class="logo">Sofa</div>
    <nav class="navigation">
      <div class="nav-item" v-for="item in list" :key="item.title">
        <NuxtLink class="link" to="/">{{ item.title }}</NuxtLink>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      list: [
        {
          title: "Home",
          src: "",
        },
        {
          title: "About",
          src: "",
        },
        {
          title: "Feature",
          src: "",
        },
        {
          title: "Contact",
          src: "",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.header {
  display: flex;
  margin: 0 auto;
  max-width: 1320px;
  padding: 20px 20px;

  .logo {
    flex: 0 0 35%;
    font-size: 40px;
    color: $TealBlue;
  }

  .navigation {
    display: flex;
    align-items: center;
    .nav-item {
      padding: 0 40px;
    }
  }
}
</style>
