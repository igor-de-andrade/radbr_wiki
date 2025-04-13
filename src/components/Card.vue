<script setup>
const props = defineProps({
  name: String,
  imgPath: String,
});
</script>

<template>
  <div class="card wide">
    <img :src="imgPath" class="card-image" />
    <span class="card-title">{{ name }}</span>
  </div>
</template>

<style scoped>
.card {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  border: solid;
  border-color: #939393;
  border-radius: 4px;
  border-width: 1px;
  width: 200px;
  padding: 10px;
  align-items: center;
  background-color: #ffffff;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
}

.card:hover {
  background-color: #e2e2e2;
  cursor: pointer;
}

.card-image {
  width: 36px;
}

.card-title {
  font-family: "Cinzel Decorative", serif;
  font-weight: 400;
  font-style: normal;
  font-size: 20px;
}
</style>
