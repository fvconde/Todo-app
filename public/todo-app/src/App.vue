<template>
  <div id="app">
    <div id="logo">
      <img src="./assets/logo.png" alt="logo">
    </div>
    
      <nav>
        <div id="tabs">
        <div>
          <router-link to="/late">Atrasado</router-link>
        </div>
        <div>
          <router-link to="/todo">A Fazer</router-link>
        </div>
        <div>
          <router-link to="/complete">Completo</router-link>
        </div> 
        </div>       
      </nav>
      <hr>
    
    
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #202D4180;
}

#logo {
  padding-right: 90%;
  padding-top: 2%;
}
 #logo img {
  height: 70px;
 }

 #tabs {
  display: flex;
  justify-content: space-around;
  flex-direction: row;
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
