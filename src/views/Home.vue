<template>
  <div class="row">
    <div class="col-2"></div>
    <div class="col-7">
      <instagram-card />
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

export default {
  name: "Home",
  components: {
    InstagramCard,
    Stories,
    sugestija,
  },
};
</script>
