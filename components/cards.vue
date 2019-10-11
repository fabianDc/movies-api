<template>
    <b-card-group deck class="mt-4"  v-if="movies.length > 0"  v-for="movie in movies" >
      <b-card
        title="{{movie.tittle}}"
        img-src="{{movie.image}}"
        img-alt="Image"
        img-top
      >
        <b-card-text>
          {{movie.description}}
        </b-card-text>
        <b-button to="/detail">View Detail</b-button>
      </b-card>
    </b-card-group>
</template>
<script>
import { mapMutations, mapState, mapActions } from 'vuex';

export default { 
    computed:{
       ...mapState('app', ['movies']), 
    },
}
</script>