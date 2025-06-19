<script setup>
</script>

<template>
    <div class="subscriptions">
  <h2>Abonnments</h2>
  <div class="subscription-item">
    <img src="/src/assets/etusa-logo.png" alt="ETUSA Logo" />
    <span class="subscription-name">ETUSA</span>
  </div>
  <div class="subscription-item">
    <img src="/src/assets/sntf-logo.png" alt="SNTF Logo" />
    <span class="subscription-name">SNTF</span>
  </div>
  <div class="subscription-item">
    <span class="material-symbols-outlined" id="icon">confirmation_number</span>
    <span class="subscription-name">Achetez des tickets</span>
  </div>
</div>
</template>

<style scoped>
.material-symbols-outlined{
  font-size: 35pt;
  color: #243A82;
  padding-right: 20px;
}
.subscriptions {
  width: 100%; /* Adjust as needed */
  margin: 0 auto;
  font-family: Arial, sans-serif;
}

h2 {
  font-size: 24px;
  margin-bottom: 20px;
  border-bottom: 2px solid #00bcd4; /* Blue underline */
  padding-bottom: 5px;
}

.subscription-item {
  display: flex;
  align-items: center;
  background-color: #e0e0e0;
  border: 1px solid #00bcd4;
  border-radius: 10px;
  padding: 10px;
  margin-bottom: 15px;
  height: 70px;
}

.subscription-item img {
  width: 50px;
  height: 50px;
  margin-right: 15px;
}

.subscription-item span.subscription-name {
  font-size: 18px;
  font-weight: bold;
}
</style>
