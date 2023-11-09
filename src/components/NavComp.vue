<template>
    <!-- 데스크탑 -->
    <div class="gnb max-w-7xl mx-auto h-20 flex justify-between items-center">
        <h1><router-link to="/">로고</router-link></h1>
        <div class="flex rounded-2xl bg-stone-200 px-5 py-1">
            <input class="basis-5/6" type="" name="" value="" placeholder="찾고싶은 사람의 닉네임을 입력해보세요">
            <button>검색</button>
        </div>
        <ul class="flex gap-20">
            <li>캘린더</li>
            <li>일기</li>
        </ul>
        <div class="myPage basis-28 text-right">
            <div v-if="loginOn === false" @click="loginOn = !loginOn">로그인</div>
            <div v-else class="flex gap-3 justify-end" @click="loginOn = !loginOn">
                <img src="../assets/img/userIcon.png" alt="default user icon" class="w-10 h-10">
                <p class="leading-10">닉네임</p>
            </div>
        </div>
    </div>
    <!-- 모바일 -->
</template>
<script setup>
import {ref} from 'vue';
 const loginOn = ref(false);
</script>
<style lang="css">
    
</style>