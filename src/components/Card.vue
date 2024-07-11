<script setup>
defineProps({
  title: String,
  imageUrl: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  handelFavorite: Function
})
</script>
<template>
  <div
    class="relative bg-white border border-grays rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
  >
    <img
      @click="handelFavorite"
      :src="!isFavorite ? '../../src/img/like-1.svg' : '../../src/img/like-2.svg'"
      alt="Like-1"
      class="absolute top-8 left-8"
    />
    <img :src="imageUrl" alt="Sneakers" />
    <p class="mt-2">Кроссовки Black Edition</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-gray">Цена:</span>
        <b>{{ price }} руб.</b>
      </div>
      <img
        @click="onClickAdd"
        :src="!isAdded ? '../../src/img/plus.svg' : '../../src/img/checked.svg'"
        alt="Plus"
      />
    </div>
  </div>
</template>
