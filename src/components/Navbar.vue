<template>
  <nav id="nav-panel">
    <div id="img-holder">
        <img src="../assets/navigation-bar.png" alt="nav-bar">
        <h1>WebDev George</h1>
    </div>
    <ul id="nav-list">
        <li v-for="item in navbarEl" :key="item.name">
          <router-link :to="item.path">{{item.name}}</router-link>
        </li>
        
    </ul>
    
  </nav>
</template>

<script>
import { ref } from "vue"


export default({
    setup() {
        const navbarEl = ref ([
            {name: 'Home', path: '/'},
            {name: 'About', path: '/about'},
            {name: 'Portfolio', path: '/portfolio'},
            {name: 'Services', path: '/services'},
            {name: 'Page', path: '/page'},
            {name: 'Contact', path: '/contact'}
        ])

        return { navbarEl }
    },
})
</script>


<style>
#nav-panel{
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: white;
    background-color: black;
}
#img-holder{
    display: flex;
    justify-content: space-around;
    flex-direction: column;
    align-items: center;
    padding: 20px;
    max-width: 100px;
    color: white
}
#img-holder img{
    max-width: 50%;
}
#img-holder h1{
    margin: 0;
    padding: 0;
    font-size: 16px;
    text-align: center;
}
#nav-list{
    display: flex;
    list-style: none;
    padding: 0;
    margin: 0;
    gap: 20px;
    margin-right: 100px;
}
#nav-list > li{
    padding: 5px;
}
</style>