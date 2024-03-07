<template>
  <div id="app">
    <div>
      <img src="./assets/logo.png" alt="logo">
    </div>
    <nav>
      <router-link to="/late" class="100px">Atrasado</router-link> |
      <router-link to="/todo">A Fazer</router-link> |
      <router-link to="/complete">Completo</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #202D4180;
}

nav {
  padding: 30px;

  a {
    // font-weight: bold;
    color: #202D4180;

    &.router-link-exact-active {
      color: #2563EB;
    }
  }
}
</style>
