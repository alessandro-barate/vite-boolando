<script>
export default {
  name: "CardComponent",
  data() {
    return {
      articles: [
        {
          id: 1,
          frontImage: "../img/1.webp",
          backImage: "../img/1b.webp",
          brand: "Levi's",
          name: "Relaxed Fit",
          price: 29.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
            {
              type: "discount",
              value: "-50%",
            },
          ],
        },
        {
          id: 2,
          frontImage: "../img/2.webp",
          backImage: "../img/2b.webp",
          brand: "Guess",
          name: "Roses Tee",
          price: 20.99,
          isInFavorites: true,
          badges: [
            {
              type: "discount",
              value: "-30%",
            },
          ],
        },
        {
          id: 3,
          frontImage: "../img/3.webp",
          backImage: "../img/3b.webp",
          brand: "Come Zucchero Filato",
          name: "Voglia di colori pastello",
          price: 129.99,
          isInFavorites: false,
          badges: [
            {
              type: "discount",
              value: "-30%",
            },
          ],
        },
        {
          id: 4,
          frontImage: "../img/4.webp",
          backImage: "../img/4b.webp",
          brand: "Levi's",
          name: "Tee Unisex",
          price: 14.99,
          isInFavorites: false,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
            {
              type: "discount",
              value: "-50%",
            },
          ],
        },
        {
          id: 5,
          frontImage: "../img/5.webp",
          backImage: "../img/5b.webp",
          brand: "Maya Deluxe",
          name: "Stripe Bodice",
          price: 99.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
            {
              type: "discount",
              value: "-50%",
            },
          ],
        },
        {
          id: 6,
          frontImage: "../img/6.webp",
          backImage: "../img/6b.webp",
          brand: "Esprit",
          name: "Maglione - Black",
          price: 29.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <div v-for="(article, index) in articles" :key="index" class="col-33-img">
    <div class="content">
      <img class="object" :src="article.frontImage" alt="" />
      <img class="object-hidden" :src="article.backImage" alt="" />
      <button class="heart bg-white top-position right-position">
        &hearts;
      </button>
    </div>
    <span
      v-for="(badge, index) in articles.badges"
      class="positioned-boxes bg-red boldness"
      >{{ articles.badge }}</span
    >
    <span class="positioned-boxes bg-green left-position boldness">{{
      articles.badge
    }}</span>
    <div>{{ article.brand }}</div>
    <div class="item-name boldness">{{ article.name }}</div>

    <!-- TODO: stampare il prezzo scontato corretto -->
    <span class="red-text boldness">14,99&euro;</span>
    <span class="text-line">{{ article.price }}&euro;</span>
  </div>
</template>
