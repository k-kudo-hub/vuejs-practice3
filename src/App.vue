<template>
  <div style="width: 700px; margin: auto; padding-top: 50px;">
    <nav>
      <router-link
        to="/" 
        active-class="link-active"
        exact
        class="link"
      >Home</router-link>
      <router-link
        to="/users"
        active-class="link-active"
        exact 
        class="link"
      >Users</router-link>
    </nav>
    <!-- URLによってコンポーネントを置き換える(動的コンポーネント) -->
    <router-view></router-view>
  </div>
</template>

<style scoped>
.link {
  margin-right: 10px;
}
.link-active {
  font-size: 20px;
}
</style>