<template>
  <div class="bg">
    <div class="profile">
      <ProfileLeft/>
      <ProfileRight/>
    </div>
    <div class="copyright">
      <span>© 2020 All rights reserved.</span>
    </div>
  </div>
</template>

<script>
import ProfileLeft from './components/ProfileLeft.vue'
import ProfileRight from './components/ProfileRight.vue'

export default {
  name: 'App',
  components: {
    ProfileRight,
    ProfileLeft
  }

}
</script>
