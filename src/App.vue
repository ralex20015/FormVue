<script>
import Login from './components/Login.vue';
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Register from './components/Register.vue';

export default {
  data(){
    return {
      hide: true,
    }
  },
  methods:{
      toggle(){
        this.hide = !this.hide;
      }
  }
  ,components: {
    Login,
    Header,
    Footer,
    Register
  },
  created(){
    this.users = localStorage.getItem("users"); 
    if(this.users){
        this.users = JSON.parse(this.users);
    }
  }
}
</script>

<template>
  <Header />
  <Login v-if="hide"/>
  <Register v-else/>
  <p v-if="hide">I don't have an <button @click="toggle">acount</button></p>
  <p v-else>I've an <button @click="toggle">acount</button></p>
  <Footer />
</template>

<style>
p{
  text-align: center;
}
</style>
