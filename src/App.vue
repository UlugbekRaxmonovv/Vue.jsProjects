<script setup>
import { onMounted } from 'vue'
import Header from './components/Header.vue'
import Drawer from './components/Drawer.vue'
import CardList from './components/CardList.vue'
import axios from 'axios'

onMounted(() => {
  console.log(123)
})

const item = [
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://static.rendez-vous.ru/files/catalog_models/resize_640x630/2/2792998_krossovki_puma_383219_sero_zelenyy_tekstil_.JPG',
    id: '1',
    title: 'Кроссовки Black Edition'
  },
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://static.rendez-vous.ru/files/catalog_models/3353184_krossovki_puma_375777_svetlo_bezhevyy_tekstil_.JPG',
    id: '2',
    title: 'Кроссовки Black Edition'
  },
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://shmotessa.ru/image/cache/catalog/ruma/novaja1/6ujgg6so5s-sfkf6dwic9odzd-hzmpgdiwdmwwo_tjtgm7kmnhnodk9ht_dwis63k5p57mppu3ijysurppmn5evn-500x500.jpg',
    id: '3',
    title: 'Кроссовки Black Edition'
  },
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ969sIxiZn_fORIMAqrU3R4w07aDjuCzPrUEoil1u8azbqvp5slD16hnVuvilwU8Urzl0&usqp=CAU',
    id: '4',
    title: 'Кроссовки Black Edition'
  },
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://images.puma.com/image/upload/f_auto,q_auto,b_rgb:fafafa/global/370716/07/fnd/RUS/w/1000/h/1000/fmt/png',
    id: '5',
    title: 'Кроссовки Black Edition'
  },
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://хасл.рф/components/com_jshopping/files/img_products/13294/puma-rs-x-13294-1.jpg',
    id: '6',
    title: 'Кроссовки Black Edition'
  },
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://shmotessa.ru/image/cache/catalog/ruma/novaja1/rb6retmoxg4hs3xyytpbnn7dqylgfjsx3coammhhqajhqmyjyhdcrzxrz6divn-xqqhc6fmgqk-gee5r44t-rztq-500x500.jpg',
    id: '7',
    title: 'Кроссовки Black Edition'
  },
  {
    name: 'name 1',
    price: 454545,
    imageUrl:
      'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ0G6IIrfK3f6jl3Ntz49jPFrqW6S2NeDtgeN0-LgiJ1Nk_kb1Ht0zeKdZxVlBSh-VJhWM&usqp=CAU',
    id: '8',
    title: 'Кроссовки Black Edition'
  }
]
</script>

<template>
  <!-- <Drawer /> -->
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-10 m">
    <Header />
    <div class="p-10">
      <div class="flex justify-between items-center">
        <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>

        <div class="flex items-center gap-5">
          <select class="py-2 px-2 border rounded-md outline-none">
            <option value="">По названию</option>
            <option value="">По цене (дешевые)</option>
            <option value="">По цене (дорогие)</option>
          </select>
          <div class="relative">
            <img class="absolute left-4 top-3" src="../src/img/search.svg" alt="" />
            <input
              class="border rounded-md py-1.5 pl-11 pr-4 outline-none focus:border-gray"
              type="text"
              placeholder="Search...."
            />
          </div>
        </div>
      </div>
      <div class="mt-10">
        <CardList :item="item" />
      </div>
    </div>
  </div>
</template>
<style></style>
