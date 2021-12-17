<template>
  <div class="card text-center">
    <div class="card-header" style="text-align: left !important">
      <div class="row">
        <div class="col-md-6">{{ info.user }}</div>
        <div class="col-md-6">{{ info.description }}</div>
      </div>
    </div>
    <div class="card-body p-0">
      <img class="card-img-top" :src="info.url" />
    </div>
    <div class="card-footer text-muted">2 days ago</div>
  </div>
</template>

<script>
export default {
  props: ["info"],
  name: "InstagramCard",
};
</script>
