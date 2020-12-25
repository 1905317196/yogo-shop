<template>
   <div class="context">
     <h1 style="margin-left:190px">注&nbsp;&nbsp;&nbsp;&nbsp;册</h1><br/>
     <div style="margin-left:150px">
        <div>请输入用户名：</div>
    <input type="text" ><br/>
    <div>请输入密码：</div>
    <input type="password" ><br/>
    <div>请确认密码：</div>
    <input type="password"><br/><br/>
     </div>
    <button @click="success()" style="margin-left:210px">提交</button>
  </div>
</template>
 
<script>
  import config from '@/config/config'
export default {
  name:'Regist',
  methods:{
    success(){
      this.$router.push('/login');
      return alert('注册成功');
    }
  }
}
</script>

<style>
.context{
  margin:110px auto;
  background:rgb(238, 234, 234);
  height:300px;
  width:450px
}
.context-nav{
  padding-top: 5%;
  padding-bottom: 5%;
  margin:0 auto;
}
</style>