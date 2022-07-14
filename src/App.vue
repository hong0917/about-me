<template>
  <div class="bg">
    <transition name="fade">
    <div class="profile" v-show="showView">
      <ProfileLeft/>
      <ProfileRight/>
    </div>
    </transition>
    
    <transition name="fade">
    <div class="copyright" v-show="showView">
      <span>© 2020 All rights reserved.</span>
    </div>
    </transition>
  </div>
</template>

<script>
import ProfileLeft from './view/ProfileLeft.vue'
import ProfileRight from './view/ProfileRight.vue'

export default {
  name: 'App',
  components: {
    ProfileRight,
    ProfileLeft
  },
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
