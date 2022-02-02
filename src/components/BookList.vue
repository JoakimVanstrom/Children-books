<template>
  <div>
      <BookCover v-for="book in books" :key="book.id" :book="book"/>
  </div>
</template>

<script>
import books from '../assets/books.json'
import BookCover from './BookCover.vue'
export default {
    components: {BookCover},
    data(){
      return{
        books: [...books]
            
    }
    }

}
</script>

<style>

</style>