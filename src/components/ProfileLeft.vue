<template>
  <div class="profile_left">
    <transition name="fade">
      <div class="site_header" v-show="showView">
        <div class="header_photo">
          <img src="../assets/img/lesser-panda.jpg" alt="photo">
        </div>
        <div class="header_title">
          <h2>Lesser_Hong</h2>
          <h4>Backend Developer</h4>
          <ul class="social-links">
            <li></li>
            <li></li>
            <li></li>
          </ul>
        </div>
        <div class="header_btn">
          <button>Contact Me</button>
        </div>
      </div>
    </transition>

    <transition name="fade" v-show="showView">
      <div class="main_menu">
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'ProfileLeft',
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
    }
  }
}
</script>

