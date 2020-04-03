<template>
  <div class="Home">
    <Card>
      <div>
        <img  class="banner" src="../assets/home-banner.png" alt="产品经理" >
      </div>
        
      
    </Card>
              
  </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.ivu-card-bordered{
  border: 0px;
}
.banner{
  width:100%; 
  height:500px;
}
</style>
