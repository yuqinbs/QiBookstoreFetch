<template>
  <div>
    <div class="book-box">
      <div class="book-image-and-info">
        <div class="book-image">
          <img
            :src="require('@/assets/images/books/' + book.imageFile)"
            :alt="book.title"
          />
          <div class="read-now-button">Read Now</div>
        </div>
        <div class="book-info">
          <div class="book-title">{{ book.title }}</div>
          <div class="book-author">{{ book.author }}</div>
          <div class="book-price">${{ (book.price / 100).toFixed(2) }}</div>
        </div>
      </div>
      <button class="cart-button">Add to Cart</button>
      <button class="buy-now-button">Buy Now</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "categoryBookListItem",
  props: {
    book: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style scoped>
.book-box {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 1em;
  max-width: 100em;
  padding: 1em;
}

.book-box img {
  align-items: center;
  max-width: 180px;
  max-height: 200px;
}

.book-image-and-info {
  display: flex;
  flex-direction: column;
  gap: 0.5em;
}

.book-title {
  margin: 0 auto;
  width: 100px;
  display: block;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.book-author {
  margin: 0 auto;
  font-size: 12px;
  width: 100px;
  display: block;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.book-image {
  width: fit-content;
}

.read-now-button {
  background-color: #0008;
  opacity: 0.5;
  color: white;
  transform: translateY(-1.6em);
  margin-bottom: -1.6em;
  text-align: center;
  padding: 0.1em;
}

.read-now-button:hover,
.buy-now-button:hover,
.cart-button:hover {
  cursor: pointer;
  opacity: 1;
}

.book-info {
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 0.25em;
}

.book-title {
  font-weight: bold;
}

.book-price {
  font-style: italic;
}

.cart-button {
  background-color: dodgerblue;
  color: white;
  padding: 0.25em 1em;

  border: solid dodgerblue 2px;
  border-radius: 7.5px;
}

.buy-now-button {
  background-color: gold;
  color: black;
  padding: 0.25em 1em;

  border: solid dodgerblue 2px;
  border-radius: 7.5px;
}
</style>
