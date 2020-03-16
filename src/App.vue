<template>
<div id="app">
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/characters">Characters</router-link>
  </div>
  <div class="content">
    <router-view />
  </div>
</div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #DDDDDD;
  height: 100%;
  width: 100%
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #DDDDDD;
}

html {
  background: url('../public/images/background.jpg') no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}


body {
  margin: 0px;
}
</style>
