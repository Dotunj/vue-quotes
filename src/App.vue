<template>
  <div class="container">
  <app-new-quote></app-new-quote>
   <app-grid :quotes="quotes"></app-grid>
  </div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue';
import NewQuote from './components/NewQuote.vue';

export default {
  data:function() {
      return{
        quotes: [
            "Just a Quote to see something",
            "Yeah for bish"
        ],
        maxQuotes: 10
      }
  },
   components:{
        appGrid: QuoteGrid,
        appNewQuote: NewQuote
      }
}
</script>

<style scoped>

</style>
