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
        </div>
        <div class="header_btn">
          <button class="call_btn" @click="copyEmail()">Contact Me</button>
        </div>
      </div>
    </transition>

    <transition name="fade" v-show="showView">
      <div class="main_menu">
        <ul class="social-links">
          <li><a href=""><img class="icon" src="../assets/img/facebook.png" alt=""></a></li>
          <li><a href=""><img class="icon" src="../assets/img/premium-icon-instagram-3991634.png" alt=""></a></li>
          <li><a href=""><img class="icon" src="../assets/img/free-icon-github-5968866.png" alt=""></a></li>
          <li><a href=""><img class="icon" src="../assets/img/back.png" alt=""></a></li>
          <li><a href=""><img class="icon" src="../assets/img/next.png" alt=""></a></li>
        </ul>
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
    },

    copyEmail(){
      alert("이메일 주소가 복사되었습니다.")
    }
  }
}
</script>

