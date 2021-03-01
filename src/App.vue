<template>
  <div id="app">
    <div id="header">
    <img src="dist/lg.png" class="lg">
  </div>
  <div id="nav">
    <ul>
      <li><router-link to="/" exact>Home</router-link></li>
       <li><router-link to="/services">Services</router-link></li>
        <li><router-link to="/about">About</router-link></li>
         <li><router-link to="/contact">Contact</router-link></li>    
    </ul>
    <div class="menu">Menu</div>
  </div>
  <div id="main">
    <router-view></router-view>
    <div id="sidebarwidget">
      <h2>Widget Title</h2>
      <hr/>
      <p>Place your wdget message here. Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here. 
      Place your wdget message here.Place your wdget message here.
      
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here.
      Place your wdget message here.Place your wdget message here. 
      Place your wdget message here.Place your wdget message here.
      </p>
    </div>
  </div>
  <div id="footer">
    Copyright &copy; Responsive Template 2021,All rights reserved.
  </div>
  </div>
</template>

<script>
import VueRouter from 'vue-router'
import Home from './pages/Home.vue'
import Services from './pages/Services.vue'
import About from './pages/About.vue'
import Contact from './pages/Contact.vue'

const routes = [
  { path: '/', component: Home },
  { path: '/services', component: Services },
  { path: '/about', component: About },
  { path: '/contact', component: Contact }
]

const router = new VueRouter({
  routes:routes,
  mode:'history'
})

export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  router:router
}
</script>

