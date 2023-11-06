<template>
    <!-- 데스크탑 -->
    <div class="gnb max-w-7xl mx-auto h-20 flex justify-between items-center">
        <ul class="flex gap-20">
            <li><router-link to="/">로고</router-link></li>
            <li>캘린더</li>
            <li>나만의 후기</li>
        </ul>
        <div>검색바</div>
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