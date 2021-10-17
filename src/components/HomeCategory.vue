<template>
  <div class="home-page">
    <section class="category-images container">
      <div class="category-image-items">
        <router-link
          style="text-decoration: none; color: inherit"
          to="../category/all"
        >
          <img
            src="@/assets/images/categories/all.jpg"
            alt="All Books"
            width="180px"
            height="180px"
          />
          <div>All Books</div>
        </router-link>
        <router-link
          style="text-decoration: none; color: inherit"
          to="../category/children"
        >
          <img
            src="@/assets/images/categories/children.jpg"
            alt="Children's Books"
            width="180px"
            height="180px"
          />
          <div>Children's</div>
        </router-link>
        <router-link
          style="text-decoration: none; color: inherit"
          to="../category/food"
        >
          <img
            src="@/assets/images/categories/food.jpg"
            alt="Food & Drink Books"
            width="180px"
            height="180px"
          />
          <div>Food & Drink</div>
        </router-link>
        <router-link
          style="text-decoration: none; color: inherit"
          to="../category/art"
        >
          <img
            src="@/assets/images/categories/art.jpg"
            alt="Art & Craft Books"
            width="180px"
            height="180px"
          />
          <div>Art & Craft</div>
        </router-link>
        <router-link
          style="text-decoration: none; color: inherit"
          to="../category/education"
        >
          <img
            src="@/assets/images/categories/education.jpg"
            alt="Education Books"
            width="180px"
            height="180px"
          />
          <div>Education</div>
        </router-link>
      </div>
    </section>
    <div class="welcome">
      <h1>Welcome to BookBook</h1>
    </div>
    <div class="trending">
      <h1>Trending</h1>
    </div>
    <section class="trending-images container">
      <div class="trending-books">
        <a>
          <img
            src="@/assets/images/books/one-hundred-reasons-to-hope.jpg"
            alt="hope"
            width="155px"
            height="200px"
          />
          <div class="buy-now">Buy Now</div>
        </a>
        <a>
          <img
            src="@/assets/images/books/big-panda-and-tiny-dragon.jpg"
            alt="panda"
            width="155px"
            height="200px"
          />
          <div class="buy-now">Buy Now</div>
        </a>
        <a>
          <img
            src="@/assets/images/books/the-primrose-railway-children.jpg"
            alt="primrose"
            width="155px"
            height="200px"
          />
          <div class="buy-now">Buy Now</div>
        </a>
        <a>
          <img
            src="@/assets/images/books/guinness-world-records-2022.jpg"
            alt="All Books"
            width="155px"
            height="200px"
          />
          <div class="buy-now">Buy Now</div>
        </a>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "HomeCategory",
};
</script>

<style scoped>
.category-image-items {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 1em;
}

.category-image-items a {
  text-align: center;
  cursor: pointer;
}

.category-image-items div {
  padding: 0.5em 0;
  background: rgba(0, 0, 0, 0.5); /* last # is percent opacity */
  color: white;
  transform: translateY(-2.25em);
  margin-bottom: -2em;
}

.welcome {
  font-size: 30px;
  text-align: center;
  margin-bottom: 10px;
  padding: 10px;
}

.trending {
  font-family: "Courier New", Courier, monospace;

  margin-left: 1.5%;
}

.trending-books {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 8em;
}

.trending-books a {
  text-align: center;
  cursor: pointer;
}

.trending-books button {
  padding: 0.5em 0;
  background: #005bff; /* last # is percent opacity */
  color: white;
  margin-top: 5px;
  margin-bottom: -2em;
}

.buy-now {
  background-color: gold;
  color: black;
  padding: 0.25em 1em;
  margin-top: 10px;
  border: solid dodgerblue 2px;
  border-radius: 7.5px;
}
</style>
