<template>
  <div class="container">
    <div class="square"></div>
      <div class="title spacing-large sides-4  ">
        THE<br>POOM<br>MAKE
      </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
:root {
  background: #ffffff;
}

.container {
  position: relative;
  margin: 0;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
 position: absolute;
font-family: Noto Sans JP;
font-style: normal;
font-weight: 500;
font-size: 5rem;
text-align: center;
color:rgb(70, 70, 70);
}

.spacing-large {
  letter-spacing:0.835em;
  padding-left: 0.835em;
}

.square {
  position: fixed;
  top: 0;
  z-index: -1;
  overflow: hidden;
  height: 100%;
  width: 5vw;
  background-color: rgb(76, 94, 255);
  justify-content: center;
}

 .sides-4 {
  background:
    linear-gradient(-90deg,currentColor 50%,#0000 0) 0 0,
    linear-gradient(currentColor 0 0) 0 0 ,
    linear-gradient(90deg,currentColor 50%,#0000 0) 100% 100%,
    linear-gradient(currentColor 0 0) 100% 100%;
  background-size: 200% 3px,3px 0%;
  background-repeat:no-repeat;
  transition: .3s,background-size .3s .3s;
}
.sides-4:hover {
  background-position: 100% 0,0 0,0 100%,100% 100%;
  background-size:200% 3px,3px 100%;
  transition: .3s,background-position .3s .3s;
 }

</style>
