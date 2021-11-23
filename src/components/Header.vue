<template>
  <div class="headermain">
      <div class="title">
      <span>Resume</span>
      </div>
      <div class="headerOpsition">
          <span class="font-large">Home</span>
          <span class="font-large">About</span>
          <span class="font-large">Contact</span>
          <i class="fas user-logo fa-user-circle"></i>
      </div>
  </div>
</template>
<script>
export default {
    name:'Header',
    data(){
        return{

        }
    }
}
</script>
<style scoped>
.headermain{
    display: flex;
    align-items: center;
    justify-content: space-around;
    background-color:  rgb(10, 10, 10, 0.9);
    height: 80px;
    width: 100%;
    color: #ffff;
    position: fixed;
    top: 0px;
    left: 00px;
}
.title{
    font-size: 25px;
    font-weight: 600;
}
.headerOpsition span{
    margin: 10px;
    cursor: pointer;
    font-weight: 600;
    /* height: 30px; */
    /* width: 30px; */
}
.headerOpsition span:hover{
    /* border: 2px solid #ffff; */
    background-color: #ffff;
    color: black;
    padding: 7px;
    border-radius: 10px;
}
.user-logo{
    font-size: 25px;
    /* padding-left: 50px; */
    margin-left: 10px;
    cursor: pointer;
    font-weight: 600;

}
</style>>