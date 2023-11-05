<template>
    <div class="relative basis-full md:basis-[48.5%] lg:basis-[31%] rounded-lg flex flex-col border shadow-md overflow-hidden">
        <div class="reviewTop basis-20 bg-yellow-400"></div>
        <div class="avatar absolute w-[45px] h-[45px] rounded-full top-14 left-5 overflow-hidden"><img class="w-[45px] h-[45px]" src="@/assets/img/userIcon.png" alt="default user icon"></div>
        <div class="reviewBottom p-5 pt-6">
            <div class="userInfo flex flex-wrap">
                <div class="basis-4/5 userName text-xl font-bold">유저이름
                    <span class="text-sm font-medium text-yellow-500"><font-awesome-icon icon="fa-solid fa-star"/> 50</span>
                </div>
                <div class="basis-1/5">
                    <button @click="likeOn=!likeOn" class=" rounded-full px-2 py-[2px] border border-rose-600" :class="likeOn === true? 'bg-rose-600 text-white':'bg-white text-rose-600'"><font-awesome-icon :icon="likeOn === true ? 'fa-solid fa-heart' : 'fa-regular fa-heart'" /> 감동</button>
                </div>
                <p class="basis-full userDesc text-sm text-stone-500 flex gap-1">
                    <span class="seperateDot">세션날짜</span>
                    <span class="seperateDot">PC명/GM</span>
                    <span>세션명</span>
                </p>
            </div>
            <div class="mt-5">
                <p class="reviewContents h-[100px]  text-stone-700 break-all line-clamp-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam, sapiente est amet blanditiis excepturi officiis, tempora ea rerum doloribus ullam laudantium magnam suscipit laboriosam temporibus quod? Aliquid ipsa officia voluptates.</p>
            </div>
            <!-- <div class="buttonArea flex justify-end gap-5">
                <button @click="likeOn = !likeOn" class="bg-rose-600 text-white rounded-full px-2 py-1"><font-awesome-icon :icon="likeOn === true ? 'fa-solid fa-heart' : 'fa-regular fa-heart'" /></button>
            </div> -->
        </div>
    </div>
</template>
<script setup>
import {ref} from 'vue';
 const likeOn = ref(false);
</script>
<style>
    
</style>