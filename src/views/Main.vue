<template>
<el-container style="height:100%">
  <el-aside width="auto"><common-aside></common-aside></el-aside>
  <el-container>
    <el-header>
      <common-header></common-header>
    </el-header>
    <common-tag/>
    <el-main>
      <router-view></router-view>
    </el-main>
  </el-container>
</el-container>
</template>

<script>
import CommonAside from '../components/CommonAside.vue'
import CommonHeader from '../components/CommonHeader.vue'
import CommonTag from '../components/CommonTag.vue'
export default {
     name:'Home',
    components:{CommonAside, CommonHeader,CommonTag},
//     mounted(){
//  this.$router.push({
//   name:'home'
//  })
//     }

}
</script>

<style lang="less" scope>
   .el-header{
    background-color:#333 ;
   }
   .el-main{
    padding-top: 0;
   }
</style>