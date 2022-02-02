<template>

    <div class="book-cover">
      <h2>{{book.title}}</h2>
      <p v-for="author in book.authors" :key="author.name">{{author.name}}</p>
    </div>
</template>

<script>
export default {
    props: ['book']

}
</script>

<style scoped lang="scss">

.book-cover {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  width: 250px;
  height: 300px;
  background-color: lightgreen;
  padding: 0 0 1.4rem 1rem;
  p, h2{
    color: white;
    margin: 0;
  }
}
</style>