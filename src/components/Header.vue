<script></script>

<template>
  <header class="flex justify-between border-b border-slate-300 px-10 py-8">
    <div class="flex items-center gap-4">
      <img src="../../src/img/logo.png" alt="logo" class="w-10" />
      <div>
        <h2 class="text-xl font-bold uppercase">Vue Sneakers</h2>
        <p class="text-slate-400">Магазин лучших кроссовок</p>
      </div>
    </div>
    <ul class="flex items-center gap-10">
      <li class="flex items-center gap-3 text-gray hover:text-black cursor-pointer">
        <img src="../img/cart.svg" alt="cart" />
        <b>1205 руб.</b>
      </li>
      <li class="flex items-center gap-3 text-gray hover:text-black cursor-pointer">
        <img src="../img/heart.svg" alt="Favorite" />
        <span>Закладки</span>
      </li>
      <li class="flex items-center gap-3 text-gray hover:text-black cursor-pointer">
        <img src="../img/profile.svg" alt="Профиль" />
        <span>Профиль</span>
      </li>
    </ul>
  </header>
</template>

<style scoped></style>
