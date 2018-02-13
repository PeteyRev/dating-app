<template>
  <div id="app">
    <header>
      <button class="mobile-toggle"><i class="fas fa-bars"></i></button>
      <nav>
        <ul class="main-nav">
          <li>
            <router-link to="/" class="button"
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
    <img src="./assets/logo.png">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto:400,500i,700');
@import "~foundation-sites/scss/foundation";
@import "/scss/app";
</style>
