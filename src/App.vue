<template>
  <div id="app">
    <div id="nav" class="container">
      <b-navbar toggleable="lg" type="dark" variant="">
        <b-navbar-brand href="#">
          <img src="@/assets/img/logo.png">
          </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ms-auto">
            <b-navbar-nav>
              <b-nav-item>
                <router-link to="/">Home</router-link>
              </b-nav-item>
               <b-nav-item>
                <router-link to="/service">service</router-link>
              </b-nav-item>
            </b-navbar-nav>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
