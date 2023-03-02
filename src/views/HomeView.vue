<template>
  <div class="block">
    <navbar />
  </div>

  <div class="block is-size-1">
    <p>
      WELCOME <br> TO <br> Moo-Waan Stationery
    </p>
  </div>

  <div class="block">
    <router-link to="/Shop" class="button is-rounded is-primary">
      SHOP
    </router-link>
  </div>

  <div class="block">
    <foot />
  </div>
</template>

<script>
// @ is an alias to /src
import navbar from '@/components/NavBar.vue';
import foot from '@/components/FooTer.vue';


export default {
  name: 'HomeView',
  components: {
    foot,
    navbar
  }
}
</script>

<style>
@import "https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css";
</style>
