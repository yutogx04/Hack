<script setup>
</script>
<template>
<div class="chatbot-container">
    <span class="material-symbols-outlined menu-icon" id="robot">robot_2</span>
    <h1>Chat bot</h1>

  <div class="chatbot-body">
    <div class="chat-input">
      <input type="text" placeholder="Posez des questions..." />
      <span class="material-symbols-outlined mic-button">mic</span>
    </div>
    <div class="chat-messages">
      <div class="message left">أين تريد الذهاب ؟</div>
      <div class="message right">الى القطب الجامعي</div>
      <div class="message left">ماهي وسيلة تنقلك ؟</div>
      <div class="message right">
        ستصل الحافلة المتجهة الى القطب الجامعي بعد 15 دقيقة يرجى الاطلاع على الخريطة
        لمعرفة تفاصيل الطريق و المدة للوصول لوجهتك
      </div>
    </div>
  </div>
</div>
</template>

<style scoped>
#robot {
  background-color: var(--accent);
        border-radius: 25%;
        margin: 7px 0;
        box-shadow: 0px 5px 5px grey;
        color: white;
        width:100px;
        height:100px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 45pt;
}
h1{
    font-weight: bold;
}
body {
  margin: 0;
  background-color: #f5f5f5;
}

.chatbot-container {
  width: 100%;
  height: 100%;
  margin: 20px auto;
  background-color: #ffffff;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.chatbot-header {
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

.chatbot-body {
  padding: 15px;
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
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.chat-messages {
  margin-top: 10px;
  display: flex;
    flex-direction: column;
}

.message {
  background-color: #f0f0f0;
  padding: 10px;
  border-radius: 10px;
  margin-bottom: 10px;
  font-size: 14px;
  width: fit-content;
}

.right{
    align-self: flex-end;
}

.left {
  align-self: flex-start;
}

.chatbot-footer {
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