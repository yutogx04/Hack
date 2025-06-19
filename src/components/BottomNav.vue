<script setup>
import { ref, computed } from 'vue'
import Index from './Index.vue';
import Abonnements from './Abonnements.vue';

const routes = {
  '/': Index,
  '/Abonnements': Abonnements,
}

const currentPath = ref(window.location.hash)

window.addEventListener('hashchange', () => {
  currentPath.value = window.location.hash
})

const currentView = computed(() => {
  return routes[currentPath.value.slice(1) || '/'] || NotFound
})
</script>

<template>
    <nav>
        <div><a href="#/Abonnements"><span class="material-symbols-outlined">card_membership</span></a></div>
        <div><a href="#/groups"><span class="material-symbols-outlined">groups</span></a></div>

        <div id="center"><a href="#/"><span class="material-symbols-outlined">add_location_alt</span></a></div>

        <div><a href="#/chatBot"><span class="material-symbols-outlined">robot_2</span></a></div>
        <div><a href="#/notifications"><span class="material-symbols-outlined">fmd_bad</span></a></div>
    </nav>
</template>



<style scoped>
    nav{
        width: calc( 90% - 20px );
        height: 100%;
        display: flex;
        flex-direction: row;
        justify-content: space-around;

        background-color: var(--accent);
        padding: 0 10px;
        margin: 0 auto;
        border-radius: 25px;

        div{
            width: 110px;
            display: flex;
            justify-content: center; /* Centers horizontally */
            align-items: center
        }
    }
    span{
        font-size: 50pt;
        margin-top: 25%;
    }
    a{
        margin:auto;
        color:white;
    }

    #center{
        background-color: white;
        border-radius: 100%;
        margin: 7px 0;
        box-shadow: 0px 5px 5px grey;
        a{
            color: var(--accent);
        }
    }
</style>