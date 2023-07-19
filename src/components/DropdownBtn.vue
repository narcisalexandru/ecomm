<template>
    <div class="container">
        <div class="button-container">
            <button class="button" @click="toggle(0)"><font-awesome-icon class="icon-rotate" icon="globe" /> Languages <font-awesome-icon icon="caret-down" /></button>
            <div class="menu" v-if="active[0]">
                <a href="#" class="links">English</a>
                <a href="#" class="links">Romanian</a>
        </div>
    </div>
    <div class="button-container">
        <button class="button" @click="toggle(1)"><font-awesome-icon icon="dollar-sign" /> Currency <font-awesome-icon icon="caret-down" /></button>
        <div class="menu" v-if="active[1]">
            <a href="" class="links">EURO</a>
            <a href="" class="links">RON</a>
        </div>
      </div>
    </div>
  </template>
  
<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  data() {
    return {
      active: [false, false] as boolean[],
    };
  },
  methods: {
    toggle(index: number) {
      this.active[index] = !this.active[index];
    },
  },
});
</script>
  
  <style scoped>
  .container {
    display: flex;
    flex-direction: row;
    gap: 25px;
  }
  
  .button-container {
    display: flex;
    flex-direction: column;
    position: relative;
  }
  
  .button {
    display: flex;
    border: 0;
    background-color: transparent;
    gap: 5px;
    color: grey;
    cursor: pointer;
  }
  
  .menu {
    display: flex;
    flex-wrap: nowrap;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    position: absolute;
    margin: 15px;
    padding: 5px;
    z-index: 1;
    background-color: white;
}
    .links {
        text-decoration: none;
        font-size: 14px;
        color: grey;
    }

    .icon-rotate {
        transform: rotate(35deg);
    }
  </style>
  