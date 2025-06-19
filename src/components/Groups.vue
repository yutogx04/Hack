<script setup>
</script>
<template>
    <div class="forum">
    <h1>Forum</h1>
    <div class="user-item">
        <div>
            <span class="material-symbols-outlined">
                account_circle
            </span>
        <span>Utilisateur1</span>
        </div>

        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta, doloribus excepturi iure, deleniti distinctio nesciunt dignissimos officiis vero repellendus quidem similique consectetur autem saepe, aspernatur repudiandae expedita itaque? Repudiandae, odit.</p>
    </div>
    <div class="user-item">
        <div>
            <span class="material-symbols-outlined">
                account_circle
            </span>
            <span>Utilisateur2</span>
        </div>

        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta, doloribus excepturi iure, deleniti distinctio nesciunt dignissimos officiis vero repellendus quidem similique consectetur autem saepe, aspernatur repudiandae expedita itaque? Repudiandae, odit.</p>
  </div>
  <div class="user-item">
    <div>
      <span class="material-symbols-outlined">
                account_circle
            </span>
      <span>Utilisateur3</span>
    </div>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta, doloribus excepturi iure, deleniti distinctio nesciunt dignissimos officiis vero repellendus quidem similique consectetur autem saepe, aspernatur repudiandae expedita itaque? Repudiandae, odit.</p>
  </div>
  <div class="user-item">
    <div>
      <span class="material-symbols-outlined">
                account_circle
            </span>
      <span>Utilisateur4</span>
    </div>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta, doloribus excepturi iure, deleniti distinctio nesciunt dignissimos officiis vero repellendus quidem similique consectetur autem saepe, aspernatur repudiandae expedita itaque? Repudiandae, odit.</p>
  </div>
  <div id="center"><button @click="(event=>{console.log('Button clicked!\nfunctionality not added')})"><span class="material-symbols-outlined">Add</span></button></div>
</div>
</template>

<style scoped>
    .forum {
  width: 382px; /* Adjust as needed */
  margin: 0 auto;
  font-family: Arial, sans-serif;
}

h1 {
  font-size: 24px;
  margin-bottom: 20px;
  border-bottom: 2px solid #000; /* Black underline */
  padding-bottom: 5px;
}

.user-item {
    display: flex;
    flex-direction: column;
  border: 1px solid #ccc;
  border-radius: 5px;
  padding: 10px;
  margin-bottom: 15px;
  div {
    display: flex;
    align-items: center;
  }
}

.user-item img {
  width: 30px;
  height: 30px;
  margin-right: 10px;
}

.user-item span {
  font-size: 16px;
  font-weight: bold;
}

 #center{
        background-color: var(--accent);
        border-radius: 100%;
        position: fixed;
        bottom: 150px;
        right: 50px;
        width: 50px;
        height: 55px;
        margin: 7px 0;
        box-shadow: 0px 5px 5px grey;
        display: flex;
        justify-content: center;
        align-items: center;
        button{
            background-color: transparent;
            border: none;

        }
        span{
            padding-top: 7px;
            font-size: 30pt;
            color: white;
        }
    }
</style>