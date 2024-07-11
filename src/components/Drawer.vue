<script setup>
import DrawrHeight from './DrawrHeight.vue'
import CardItemList from '../components/CardItemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-screen w-full m-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
    <DrawrHeight />

    <CardItemList />

    <div class="flex flex-col gap-5 mt-7">
      <div class="flex gap-2">
        <span>Итого:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b> 29999 ₽</b>
      </div>
      <div class="flex gap-2">
        <span>Налог 5%:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b> 1500 ₽</b>
      </div>
      <button
        class="mt-7 bg-lime w-full rounded-xl py-3 text-white transition active:bg-green disabled:bg-bermuda"
      >
        Buyurtma berish
      </button>
    </div>
  </div>
</template>
