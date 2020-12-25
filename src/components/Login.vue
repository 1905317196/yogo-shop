<template>
  <div class="context">
    <div class="context-nav"><h1 style="margin-left:190px;">登&nbsp;&nbsp;&nbsp;&nbsp;录</h1></div>
      <Input prefix="md-person" placeholder="邮箱/手机/用户名"
       style="width:200px;margin-left:125px;margin-bottom:30px;margin-top:30px" size="large" v-model="username"/>
      <br>
      <Input prefix="md-lock" placeholder="请输入密码" type="password" style="width:200px;margin-left:125px;margin-bottom:15px" size="large" v-model="password" />
    <div>
      <router-link to="/regist" style="color:#000;float:right;margin-right:40px">注册</router-link>
    </div>   
    <Button to="/"  @click="loginSubmit()" type="success"
    long style="margin-left:200px;width:50px;margin-top:30px;" size="large">登录</Button>
    <!-- -->
  </div>
</template>

<script>
import config from '@/config/config'
export default{
  name: 'Login',
  data(){
    return{
      logname:'',
      password:''
    }
  },
  methods:{
    loginSubmit(){
      this.$router.push('/');
      return alert("登录成功");
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