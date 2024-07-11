<script setup>
import Card from './Card.vue'
const onClickAdd = () => {
  alert('swfrvg')
}
defineProps({
  item: Array
})
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      v-for="item in item"
      :key="item.id"
      :title="item.title"
      :imageUrl="item.imageUrl"
      :price="item.price"
      :onClickAdd="onClickAdd"
    />
  </div>
</template>
