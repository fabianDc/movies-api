<template>
  <div class="container">
    <cards v-if="movies"></cards>
  </div>
</template>

<script>
import { mapState } from 'vuex'
import Logo from "~/components/Logo.vue"
import cards from '../components/cards.vue';

export default {
  layout: 'layouts/default',
  components: {
    Logo,
    cards,
  }
};
</script>

<style>

</style>
