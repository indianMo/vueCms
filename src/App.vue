<template>
   
  <div id="app">
    <router-view  v-loading.fullscreen.lock="loadingStatus"></router-view>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
export default {
  name: 'app',
  computed: {
    ...mapGetters([
       'loadingStatus'
    ])
  },
  data () {
    return {
    }
  },
  created: function () {
    // this.fullscreenLoading = true
  }
}
</script>
<style>
   form input[type=text]{
     width:420px;
   }
</style>
