<template>
  <div class="profile_left">
      <div class="site_header">
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

      <div class="main_menu">
        <ul class="social-links">
          <li><a href=""><img class="icon" src="../assets/img/facebook.png" alt="facebook_icon"></a></li>
          <li><a href=""><img class="icon" src="../assets/img/premium-icon-instagram-3991634.png" alt="instagram_icon"></a></li>
          <li><a href=""><img class="icon" src="../assets/img/free-icon-github-sign-25657.png" alt="github_icon"></a></li>
          <li><a href=""><img class="icon" src="../assets/img/back.png" alt="back_icon"></a></li>
          <li><a href=""><img class="icon" src="../assets/img/next.png" alt="next_icon"></a></li>
        </ul>
      </div>
  </div>
</template>

<script>
export default {
  name: 'ProfileLeft',
  data(){
    return{
    
    }
  },
  methods:{
    copyEmail(){
      alert("이메일 주소가 복사되었습니다.")
    }
  }
}
</script>

