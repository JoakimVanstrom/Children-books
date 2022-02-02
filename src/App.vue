<template>
  <div id="app">
        <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/singlebook">single book</router-link> |
    </div>
      <div class="readinglist">
      <router-link to="/ReadingList">Reading List</router-link>

      </div>
    <router-view/>
  </div>
</template>

<script>


export default {
  
  data(){
    return{
  
    }
  },
created(){
  // fetch('https://gutendex.com/books')
  // .then((response) => response.json())
  // .then((data) => (this.$root.books.push(data.results)))
  // this.$root.books.push(books)
},


}
</script>

<style lang="scss">

</style>

