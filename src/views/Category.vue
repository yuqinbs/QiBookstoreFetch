<template>
  <div>
    <category-nav></category-nav>
    <category-book-list :books="books"> </category-book-list>
  </div>
</template>

<script>
import CategoryNav from "@/components/CategoryNav";
import CategoryBookList from "@/components/CategoryBookList";

export default {
  name: "category",
  components: {
    CategoryNav,
    CategoryBookList,
  },
  data: function () {
    return {
      books: [
        {
          bookId: 1001,
          title: "How to Save a Life: The Inside Story of Grey's Anatomy",
          imageFile: "save.jpg",
          author: "Lynette Rice",
          price: 1628,
          isPublic: true,
        },
        {
          bookId: 1002,
          title: "Together: Memorable Meals, Made Easy",
          imageFile: "together.jpg",
          author: "Jamie Oliver",
          price: 1320,
          isPublic: false,
        },
        {
          bookId: 1003,
          title: "One Hundred Reasons To Hope",
          imageFile: "hope.jpg",
          author: "Adam Larkum",
          price: 999,
          isPublic: true,
        },
        {
          bookId: 1004,
          title: "The Primrose Railway Children",
          imageFile: "primrose.jpg",
          author: "Jacqueline Wilson",
          price: 649,
          isPublic: true,
        },
        {
          bookId: 1005,
          title:
            "Big Panda and Tiny Dragon: The beautifully illustrated and comforting story of friendship as seen on ITV News",
          imageFile: "panda.jpg",
          author: "James Norbury",
          price: 1299,
          isPublic: true,
        },
        {
          bookId: 1006,
          title: "Guinness World Records 2022",
          imageFile: "record.jpg",
          author: "Guinness World Records",
          price: 1028,
          isPublic: true,
        },
      ],
    };
  },
};
</script>

<style scoped></style>
