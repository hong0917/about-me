<template>
  <div class="profile_right">
    <transition name="fade">
      <div class="site_content" v-show="showView">

      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'ProfileRight',
  data(){
    return{
      showView:false
    }
  },
  mounted(){
    setTimeout(this.changeView,500)
  },
  methods:{
    changeView(){
        this.showView = !this.showView
    },
  }
}
</script>

<style >

</style>
