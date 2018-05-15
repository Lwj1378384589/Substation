<template>
    <div id="index">
      <my-header></my-header>
      <!-- <my-aside></my-aside> -->
      <router-view class="view"> </router-view>
      <my-footer></my-footer>
    </div>
</template>

<script>
import MyHeader from '@/components/frame/header'
import MyFooter from '@/components/frame/footer'
import MyAside from '@/components/frame/aside'
export default {
  name: 'index',
  data () {
    return {
    }
  },
  components:{MyHeader,MyFooter,MyAside}
}
</script>

<style scoped>
  

</style>
