/* eslint-disable */
<template>
  <div id="app">
    <header>
      <button @click="toggleMenu" ref="mobilemenu" class="mobile-toggle"><i class="fas fa-bars"></i></button>
      <nav>
        <ul class="main-nav">
          <li>
            <router-link to="/HelloWorld" class="button"
            active-class="active">link 1</router-link>
          </li>
          <li>
            <router-link to="/" class="button"
            active-class="active">link 2</router-link>
          </li>
          <li>
            <router-link to="/" class="button"
            active-class="active">link 2</router-link>
          </li>
        </ul>
        </nav>
    </header>
    <img src="./assets/harr.jpg">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  methods: {
    toggleMenu () {
      let menu = this.$refs.mobilemenu.nextElementSibling
      menu.classList.toggle('open')
    }
  }
}
</script>
<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Roboto:400,500i,700");
@import "~foundation-sites/scss/foundation";
@import "/scss/app";
</style>
