<template>
    <div class="relative basis-full md:basis-[31.7%] lg:basis-[23.7%] rounded-lg flex flex-col border shadow-md overflow-hidden">
        <div class="reviewTop basis-16 bg-yellow-400"></div>
        <div class="avatar absolute w-10 h-10 rounded-full top-10 left-5 overflow-hidden"><img src="@/assets/img/userIcon.png" alt="default user icon"></div>
        <div class="reviewBottom p-5">
            <div class="userInfo">
                <p class="userName text-xl font-bold">유저이름
                    <span class="text-sm font-medium text-yellow-500"><font-awesome-icon icon="fa-solid fa-star"/> 50</span>
                </p>
                <p class="userDesc text-sm text-stone-500">자기소개멘트 어쩌구저쩌구</p>
            </div>
            <div class="mt-5">
                <p class="reviewContents text-stone-800 line-clamp-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam, sapiente est amet blanditiis excepturi officiis, tempora ea rerum doloribus ullam laudantium magnam suscipit laboriosam temporibus quod? Aliquid ipsa officia voluptates.</p>
            </div>
            <div class="buttonArea flex justify-end gap-5">
                <button @click="likeOn = !likeOn" class="bg-rose-600 text-white rounded-full px-2 py-1"><font-awesome-icon :icon="likeOn === true ? 'fa-solid fa-heart' : 'fa-regular fa-heart'" /></button>
            </div>
        </div>
    </div>
</template>
<script setup>
import {ref} from 'vue';
 const likeOn = ref(false);
</script>
<style>
    
</style>