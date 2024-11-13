<template>
  <div class="card" style="width: 18rem">
    <img :src="imageSrc" class="card-img-top" alt="Card image" />
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <a :href="link" class="btn btn-link">Read More →</a>
    </div>
  </div>
</template>

<script setup>
defineProps({
  imageSrc: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  link: {
    type: String,
    required: true,
  },
});
</script>

<style scoped>
.card-title {
  font-size: 1.25rem;
  font-weight: bold;
}
.btn-link {
  color: #007bff;
  text-decoration: none;
}
.btn-link:hover {
  text-decoration: underline;
}
</style>
