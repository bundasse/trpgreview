<template>
  <div class="wrapper max-w-7xl mx-auto px-[2%] lg:px-0 flex flex-wrap">
    <div class="basis-full my-5 flex justify-between">
      <h2 class="text-4xl font-bold my-5">내가 받은 후기</h2>
      <button class="text-stone-500" @click.prevent>더보기<span class="text-stone-400"><font-awesome-icon icon="fa-solid fa-angle-right" /></span></button>
    </div>
    <div class="reviewList basis-full flex flex-wrap gap-[25px]">
      <CommentComp v-for="(e,i) in 10" :key="i" />
    </div>
    <div class="basis-full my-5 flex justify-between">
      <h2 class="text-4xl font-bold my-5">내가 남긴 후기</h2>
      <button>더보기</button>
    </div>
    <div class="reviewList basis-full flex flex-wrap gap-[25px]">
      <CommentComp v-for="(e,i) in 10" :key="i" />
    </div>
  </div>
</template>

<script setup>
import CommentComp from '@/components/CommentComp.vue';
</script>
