<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
  <div class="reviewList max-w-7xl mx-auto px-[2%] lg:px-0 flex flex-wrap gap-5">
    <CommentComp v-for="(e,i) in 10" :key="i" />
  </div>
</template>

<script>
import CommentComp from '@/components/CommentComp.vue'
export default {
  name: 'HomeView',
  components: {
    CommentComp
  }
}
</script>
