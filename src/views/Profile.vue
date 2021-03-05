<template>
  <div class="profile">
      <div class="container">
          <div class="row justify-content-center" >
              <div class="col-lg-6">
                <div class="media text-left">
                <img src="../assets/avatar5.png" class="user-pic mr-3">
                <div class="media-body">
                    <h5 class="mt-0">{{ firstName }} {{ lastName }}</h5>
                    <h6 class="MT-0">{{ ask1 }} {{ daerah }}</h6>
                    <h6 class="MT-0">{{ask2}} {{ hobby }}</h6>
                </div>
                </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>

import 'bootstrap/dist/css/bootstrap.css'

export default {
  name: 'profile',
  data: function(){
      return{
          firstName: 'No Name',
          lastName: 'UNKNOW',
          daerah: 'Belahan Bumi',
          hobby: 'No Hobby',
          ask1: 'daerah :',
          ask2: 'hobby  :'
      }
  },
  components: {
    
  }
}
</script>

<style scoped>
.user-pic{
    border-radius: 200%;
    height: 80px;
    width: 80px;

}
</style>
