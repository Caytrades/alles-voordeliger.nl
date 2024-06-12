<script setup>
import LoadingAnimation from '../components/LoadingAnimation.vue'

</script>



<template>
    <div class="container">
      <transition name="fade" v-for="(item, i) in items" :key="i">
        <div class="loading" v-show="item.loading">
            <LoadingAnimation/>
        </div>
      </transition>
    
      <transition name="fade">
        <div class="success-animation" v-show="!items.some(item => item.loading)">
          <div class="success-message">
            Success! Your task has been completed.
          </div>
        </div>
      </transition>
    </div>
  </template>


<script>
  export default {
    data() {
      return {
        items: []
      };
    },
    mounted() {
      this.simulateLoading();
    },
    methods: {
      simulateLoading() {
        this.items = [];
        for (let i = 0; i < 2; i++) {
          this.items.push({ loading: true });
          setTimeout(() => {
            this.items[i].loading = false;
          }, (i + 1) * 1000); // Delay each loading completion by 1 second
        }
      }
    }
  };
  </script>
  

  
  <style scoped>
  .container {
    text-align: center;
  }


  .success-animation{
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}

.success-message {
    padding: 20px;
    background-color: #4CAF50;
    color: white;
    border-radius: 5px;
    animation: fadeIn 0.5s 5s forwards, fadeOut 5s 10s forwards;
}
  
  .loading, .success {
    padding: 20px;
    color: white;
    border-radius: 5px;
    margin-bottom: 20px;
    opacity: 0;
    transition: opacity 0.5s;
  }
  
  .fade-enter-active, .fade-leave-active {
    transition: opacity 2s;
  }
  
  .fade-enter, .fade-leave-to {
    opacity: 5;
  }
  

@keyframes fadeIn {
    0% {opacity: 1;}
    100% {opacity: 0;}
}

@keyframes fadeOut {
    0% {opacity: 1;}
    100% {opacity: 0;}
}
  </style>
  