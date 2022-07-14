<template>
  <div class="profile_right">
    <transition name="fade">
      <div class="site_content" v-show="showView">
        <Intro></Intro>
        <Portpolio></Portpolio>
      </div>
    </transition>
  </div>
</template>

<script>
import Intro from '../components/Intro.vue'
import Portpolio from '../components/Portpolio.vue' 

export default {
  name: 'ProfileRight',
  data(){
    return{
      showView:false
    }
  },
  components:{
    Intro,
    Portpolio
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

<style>

</style>
