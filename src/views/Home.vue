<template>
  <div>
        <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/singlebook">single book</router-link> |
      <router-link to="/ReadingList">Reading List</router-link>
    </div>
    
    <div id="wrapper">
    <h1>Classic Childrens books</h1>
    <BookList class="all-books" />
    </div>
  </div>
</template>


<script>
import books from '../assets/books.json'
import BookList from '../components/BookList.vue'
export default {
  components: {BookList},
    data(){return{
    books: [...books]
}},
provide(){
  return {
    books: this.books
  }
}
}

</script>


<style lang="scss">
#wrapper {
  padding-top: 4rem;
  h1 {
    padding-left: 1rem;
  }
}
.all-books{
  padding-top: 3rem;
  display: grid;
  place-items: center;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(2,1fr);
  grid-gap: 1rem;

}

</style>
