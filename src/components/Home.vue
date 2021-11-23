<template>
  <div>
      <SideBar></SideBar>
      <Header></Header>
  </div>
</template>
<script>
import SideBar from '../components/SideBar.vue'
import Header from '../components/Header.vue'
export default {
    name:'Home',
    components:{
        SideBar,
        Header,
    },
    data(){
        return{

        }
    }
}
</script>
<style scoped>
</style>