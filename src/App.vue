<template>
  <div id="app">
    <div id="nav">
      <ul class="flex-1 flex justify-evenly items-center">
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/dogs">Dogs</router-link></li>
        <li><router-link to="/search">Search</router-link></li>
        <li><router-link to="/my-favourites">Favourites</router-link></li>
      </ul>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: "Poppins", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 10px;
  background: var(--color-primary);
  color: var(--color-tertiary);
}

#nav a.router-link-exact-active {
  color: #fff;
}
</style>
