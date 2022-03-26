<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
<div class="home">
    <div class="header">
      <h2>Hi <b>Client!</b></h2> 
      <br> 
      <div class="input">
         <input type="text" placeholder="find what you want..." > <i class="bx bx-search"></i>
        </div>
        <div class= "combo-header">
        
           
           <br>
          <h3>Arma tu combo</h3>
           <p >Pan de sabor y topping <br> </p>
          </div>
          <div class="img">
            <img src="https://walnuts.org/wp-content/uploads/2017/09/e946dc4d9fe2d2b-0AF7FFD6-06D4-44DC-8CE62D98DC6ACCD8-900x600.jpg" alt="cake" height="200" width="200">
          </div>
          <div class="myDiv">
                <div :key="index" class="avatar" v-for="(item, index) in 1">
                  <i class= 'bx bxs-cake bx-sm'></i>
                </div>
                &nbsp 
                &nbsp 
                 <div :key="index" class="avatar" v-for="(item, index) in 1">
                  <i class= 'bx bx-lemon bx-sm'></i>
                </div>
                &nbsp 
                &nbsp 
                 <div :key="index" class="avatar" v-for="(item, index) in 1">
                  <i class= 'bx bx-cheese bx-sm'></i>
                </div>
                &nbsp 
                &nbsp 
                 <div :key="index" class="avatar" v-for="(item, index) in 1">
                  <i class= 'bx bxs-coffee-togo bx-sm'></i>
                </div>
             </div>
                 
    </div>
  </div>
   <div id="app">
      <div class="navbar-container">
        <div class="navbar-content">
          
        </div>
      </div>
      <router-view></router-view>
   </div>
   <footer>
     <h3> Pastelería YUm YUm</h3> 
    <div class="img" align= "center">
      <img src="https://miralogos.com/wp-content/uploads/2020/03/Logo-pasteleria-yum-yum.jpg" alt="cake" height="500" width="600">
      <h3>Ensenada, Baja California</h3>
       <h3>Informes y pedidos al teléfono 646 2358789</h3>    
    </div>
   </footer>
</template>

<style>
.index {
  display: flex;
  border-radius: 10px;
}
 .myDiv {
   display: flex;
  justify-content: center;
  padding: 20px;
  justify-myDiv: space-between;
 }
.home {
   .scroll-menu {
    .scroll-content {
      .avatar {
        padding: 10px;
      }
    }
  }
}
.navbar-container{
  width: 100%;
  position: fixed;
  bottom: 0;
  .navbar-content{
    padding: 20px;
    display: flex;
    justify-content: space-between;
    a{
   &.router: link exact active; {
      color: rgba(255, 131, 62);
    }
    }
  }
}
 
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
   text-align: center;

  }
*{
  margin: 0px;
  padding: 0px;

}
 .combo-header {
   background-color: rgba(74,174,84);
   color: white;
   padding: 10px;
   width: 100%;
   border-radius: 80px;
   
 }
   
 
</style>
