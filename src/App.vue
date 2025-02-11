<script setup>
import { ref } from 'vue'
import HelloWorld from './components/HelloWorld.vue'

// 删除账号函数
const deleteAccount = () => {
  alert('Account deleted successfully!')
}
</script>

<template>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header> -->

  <!-- 删除账号按钮 -->
  <div class="delete-container">
    <button class="delete-button" @click="deleteAccount">Delete Account</button>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

.delete-container {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

.delete-button {
  background-color: #ff4d4d;
  color: white;
  border: none;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  border-radius: 5px;
  transition: background 0.3s;
}

.delete-button:hover {
  background-color: #cc0000;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
