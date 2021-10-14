<template>
  <nav class="category-nav">
    <ul class="category-buttons">
      <li class="button selected-category-button">All Books</li>
      <router-link
        to="children"
        tag="li"
        class="button unselected-category-button"
      >
        Children's
      </router-link>
      <router-link to="food" tag="li" class="button unselected-category-button">
        Food & Drink
      </router-link>
      <router-link to="art" tag="li" class="button unselected-category-button">
        Art & Craft
      </router-link>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "CategoryNav",
};
</script>

<style scoped>
.category-buttons {
  display: flex;
  flex-direction: row;
  text-align: center;
  background-color: var(--neutral-color);
}

.button.selected-category-button {
  background-color: var(--primary-color);
}

.button.unselected-category-button,
.button.unselected-category-button:visited {
  background-color: var(--neutral-color);
}

.button.unselected-category-button:hover,
.button.unselected-category-button:active {
  background-color: var(--primary-color);
}
</style>
