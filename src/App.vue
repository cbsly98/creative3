<template>
<div id="app">
  <div id="content-wrap">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/characters">Characters</router-link>
    </div>
    <div class="content">
      <router-view />
    </div>
  </div>
  <div class="footer">
    <a href="https://github.com/cbsly98/creative3">Github</a>
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
  min-height: 100vh;
  width: 100%;
  position: relative;
}

#content-wrap {
  padding-bottom: 2.5rem;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #DDDDDD;
}

#nav a.router-link-exact-active {
  color: #F2921D;
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

.footer {
  width: 100%;
  background: #F2921D;
  text-align: center;
  position: absolute;
  bottom: 0;
}
</style>
