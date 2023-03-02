<template>
    <div class="block">
        <navbar />
    </div>

    <div class="block is-size-1 has-text-centered">
        All Item
    </div>

    <div class="block">
        <ItemCard />
    </div>

    <div class="block">
        <foot />
    </div>
</template>


<style>
@import "https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css";
</style>

<script>
// @ is an alias to /src
import navbar from '@/components/NavBar.vue';
import foot from '@/components/FooTer.vue';
import ItemCard from '@/components/ItemCard.vue';

export default {
  name: 'HomeView',
  components: {
    foot,
    navbar,
    ItemCard
  }
}
</script>