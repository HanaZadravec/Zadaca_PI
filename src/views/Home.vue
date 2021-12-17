<template>
  <div class="row">
    <div class="col-2"></div>
    <div class="col-7">
      <instagram-card
        v-for="card in filteredCards"
        :key="card.url"
        :info="card"
      />
    </div>
    <div class="col-3">
      <Stories />
      <Stories />
      <Stories />
    </div>
  </div>
  <div class="row">
    <div class="col-2"></div>
    <div class="col-7" style="margin-top: 20px; display: flex">
      <sugestija />
      <sugestija />
      <sugestija />
      <sugestija />
      <sugestija />
    </div>
    <div class="col-3"></div>
  </div>
</template>

<script>
import InstagramCard from "@/components/InstagramCard.vue";
import Stories from "@/components/Stories.vue";
import sugestija from "@/components/sugestija.vue";
import store from "@/store.js";

export default {
  name: "Home",
  data: function () {
    return {
      cards: [
        {
          url: "https://picsum.photos/id/2/400/400",
          description: "laptop",
          user: "Hana Zadravec",
        },
        {
          url: "https://picsum.photos/id/1/400/400",
          description: "laptop#2",
          user: "Matija Zadravec",
        },
        {
          url: "https://picsum.photos/id/3/400/400",
          description: "laptop#3",
          user: "Marina Lovac",
        },
      ],
      store,
    };
  },
  computed: {
    filteredCards() {
      let termin = this.store.searchTerm;
      let newCards = [];
      for (let card of this.cards) {
        if (
          card.description.toLowerCase().indexOf(termin.toLowerCase()) >= 0 ||
          card.user.toLowerCase().indexOf(termin.toLowerCase()) >= 0
        ) {
          newCards.push(card);
        }
      }
      return newCards;
    },
  },
  components: {
    InstagramCard,
    Stories,
    sugestija,
  },
};
</script>
