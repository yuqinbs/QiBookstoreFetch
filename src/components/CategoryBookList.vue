<template>
  <div class="book-boxes">
    <category-book-list-item :book="books[0]"></category-book-list-item>
    <category-book-list-item :book="books[1]"></category-book-list-item>
    <category-book-list-item :book="books[2]"></category-book-list-item>
    <category-book-list-item :book="books[3]"></category-book-list-item>
    <category-book-list-item :book="books[4]"></category-book-list-item>
    <category-book-list-item :book="books[5]"></category-book-list-item>
  </div>
</template>

<script>
import CategoryBookListItem from "./CategoryBookListItem";

export default {
  name: "CategoryBookList",
  props: {
    books: {
      type: Array,
      required: true,
    },
  },
  components: {
    CategoryBookListItem,
  },
};
</script>

<style scoped>
.book-boxes {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 1em;
  max-width: 100em;
  padding: 1em;
  flex-wrap: wrap;
}
</style>
