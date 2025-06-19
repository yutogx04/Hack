<script setup>
</script>
<template>
    <div class="app-container">
  <div class="section">
    <div class="section-header">
      <span class="section-number">1</span>
      <h2>Specifiez votre itineraire</h2>
    </div>
    <div class="route-selection">
      <div class="route-item">
        <span>Debut</span>
        <select class="add-button" placeholder="Choisissez une station">
            <option value="station1">Station 1</option>
            <option value="station2">Station 2</option>
            <option value="station3">Station 3</option>
        </select>
        <button class="plus-button">+</button>
      </div>
      <div class="route-item">
        <span>Fin</span>
        <select class="add-button" placeholder="Choisissez une station">
            <option value="station1">Station 1</option>
            <option value="station2">Station 2</option>
            <option value="station3">Station 3</option></select>
        <button class="plus-button">+</button>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-header">
      <span class="section-number">2</span>
      <h2>Demarrez un itineraire</h2>
    </div>
    <div class="map-and-info">
      <div class="map-container">
        <img src="@/assets/asset2.png" alt="Map" />
      </div>
      <div class="info-container">
        <div id="input">
            <span class="material-symbols-outlined menu-icon" id="robot">robot_2</span>
        <div class="chat-input">
      <input type="text" placeholder="Posez des questions..." />
      <span class="material-symbols-outlined mic-button">mic</span>
        </div>
    </div>
        <div class="station-info">
          <h3>Informations sur les stations</h3>
          <div class="info-item">
            <img src="@/assets/asset3.png" alt="Station Icon" />
            <img src="@/assets/asset3.png" alt="Station Icon" />
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>
<style scoped>
#input{
    display: flex;
    flex-direction: row;
}
#robot {
  background-color: var(--accent);
        border-radius: 100%;
        margin: 7px 0;
        box-shadow: 0px 5px 5px grey;
        color: white;
        width:40px;
        height:40px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 20pt;
}
h2{
    font-weight: bold;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  background-color: #f5f5f5;
}

.app-container {
  width: 100%;
  height: 100%;
  margin: 20px auto;
  background-color: #ffffff;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.app-header {
  display: flex;
  align-items: center;
  padding: 10px 15px;
  background-color: #00bfa5;
  color: #ffffff;
}

.menu-icon {
  font-size: 20px;
  margin-right: 10px;
}

.search-bar {
  flex: 1;
  padding: 5px;
  border: none;
  border-radius: 5px;
}

.section {
  padding: 15px;
  border-bottom: 1px solid #ccc;
}

.section-header {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.section-number {
  background-color: #00bfa5;
  color: #ffffff;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-right: 10px;
}

.route-selection {
  display: flex;
  justify-content: space-around;
}

.route-item {
  display: flex;
  align-items: center;
}

.add-button {
  margin-left: 10px;
  background-color: #f0f0f0;
  border: none;
  border-radius: 5px;
  padding: 5px 10px;
  cursor: pointer;
}

.plus-button {
  margin-left: 5px;
  background-color: #00bfa5;
  color: #ffffff;
  border: none;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.map-and-info {
  display: flex;
  gap: 10px;
}
.map-container {
  width: 50%;

  height: 230px;
  overflow: auto;
}
.map-container img {
  border: 1px solid #ccc;
}

.info-container {
  flex: 1;
}

.chat-input {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
  flex: 1;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 20px;
  outline: none;
}

.chat-input input {
  width: 100%;
    border: none;
    color: transparent;
}

.mic-button {
  margin-left: 10px;
  background-color: #00bfa5;
  color: #ffffff;
  border: none;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.station-info h3 {
  margin-bottom: 5px;
}

.info-item {
  margin-bottom: 10px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  img {
    width: 50%;
  }
}

.app-footer {
  display: flex;
  justify-content: space-around;
  padding: 10px;
  background-color: #00bfa5;
}

.footer-button {
  background-color: #ffffff;
  border: none;
  border-radius: 50%;
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}
</style>