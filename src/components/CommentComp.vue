<template>
    <div class="basis-1/5 padding-5 rounded-md flex flex-col">
        <div class="reviewTop">상단배너</div>
        <div class="avatar w-10 rounded-full"><img src="" alt=""></div>
        <div class="reviewBottom">
            <p class="reviewName"></p>
            <p class="reviewContents"></p>
        </div>
        <button @click.prevent>좋아요</button>
    </div>
</template>
<script setup>
const reviews = ref([]);

</script>
<style>
    
</style>