<script setup>

</script>
<template>
    <nav>
        <a href="#">
            <span class="material-symbols-outlined">
                menu
            </span>
        </a>
        <div id="search">
            <input type="text">
            <span class="material-symbols-outlined">
                search
            </span>
        </div>
        <a href="#">
            <span class="material-symbols-outlined">
                account_circle
            </span>
        </a>
    </nav>
    
</template>

<style scoped>
    nav{
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        background: var(--accent);
        position: sticky;
        align-items: center;
        padding: 2px;
        a,span{
        color: var(--grey);
    }
    }
    span{
        font-size:30pt;
    }
    #search {
        display: flex;
        align-items: center;
        background: var(--light-grey);
        width: 80%;
        input{
            width: 100%;
            border: none;
            background: transparent;
        }
    }
</style>