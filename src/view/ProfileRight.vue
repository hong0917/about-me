<template>
  <div class="profile_right">
      <div class="site_content">
        <Intro></Intro>
        <Portpolio></Portpolio>
      </div>
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
}
</script>

<style>

</style>
