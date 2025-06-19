<script setup>
import NavBar from './components/NavBar.vue';
import BottomNav from './components/BottomNav.vue';
import Index from './components/Index.vue';
import Abonnements from './components/Abonnements.vue';
import NotFound from './components/NotFound.vue';
import Groups from './components/Groups.vue';
import chatBot from './components/chatBot.vue';
import Notifications from './components/Notifications.vue';

import {ref,computed} from 'vue'

const showDiv = ref(true)



const routes = {
  '/': Index,
  '/Abonnements': Abonnements,
  '/groups': Groups,
  '/chatBot': chatBot,
  '/notifications': Notifications,
}

const currentPath = ref(window.location.hash)

window.addEventListener('hashchange', () => {
  currentPath.value = window.location.hash
})

const currentView = computed(() => {
  return routes[currentPath.value.slice(1) || '/'] || NotFound
})

console.log(currentPath.value.slice(1))
</script>

<template>
  <div id="loading" v-if="showDiv">
    <span class="material-symbols-outlined">
      commute
    </span>
    <img src="./assets/logo.svg" alt="logo">
    <button @click="(event)=>{showDiv=false;}">Commencez</button>
  </div>
  <div id="wrapper">
    <header>
      <navBar/>
    </header>
    <main>
       <component :is="currentView" />
    </main>
    <footer>
      <BottomNav/>
    </footer>
  </div>
</template>

<style scoped>
.material-symbols-outlined {
  color: white;
  font-size: 25vw;
}
#loading{
  background: var(--accent);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: fixed;
  z-index: 20;
  width:100%;
  height:100%;
  img{
    width: 50%;
  }
  span{
    width: 25%;
  }
  button{
    border-radius: 5px ;
    margin-top: 25%;
    background-color: var(--light-grey);
    color: var(--accent);
    box-shadow: 0px 5px 5px gray;
    height: 5%;
    width: 50%;
    border: 1px solid var(--light-grey) ;
    font-size: 5vw;
  }
}

main {
  flex: 1; /* Makes the middle row take all available space */
  overflow-y: auto; /* Enables scrolling */
}
header{
  height: 60px;
}
footer{
  margin-bottom: 15px;
  height: 110px;
}


#wrapper{
  display: flex;
  flex-direction: column;
  height: 100%;
}
</style>