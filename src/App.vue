<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">
        Home
      </router-link> |
      <router-link to="/about">
        About
      </router-link> |
      <router-link to="/add-category">
        辞書登録
      </router-link>
    </div>
    <router-view />
  </div>
</template>

<style>
@import 'HTML5_Doctor_CSS Reset.css';
* {
  box-sizing: border-box;
  font-family: "Yu-Gothic",sans-serif;
  color: #333;
}
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
