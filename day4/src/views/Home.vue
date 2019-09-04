<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->

    <ul v-for="(item,index) in Arr" :key="index" @click="run">
      <li>{{item}}</li>
    </ul>
    <span>1231</span>
<!-- （2）可以进行数据的遍历（20分）
（3）提交git
（4）使用git进行代码管理（20分）
（5）创建出自己的分支（20分） -->
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
 data(){
   return {
     Arr:["a","2","5g","h"]
   }
 },
 methods:{
   run(){
     this.Arr.forEach((item=>{
       console.log(item)
     }))
   }
 }
}
</script>
