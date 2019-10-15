<template>
 <div>
  <div class="title">
  </div>
  <div class="container">
  <div class="flower">
  </div>
  <div class="label">
  <h1 class="title">Phloxus Farms</h1>
  <h3 class="subtitle">- Shelton, WA -</h3>
  </div>
  <div class="background-bar">
  </div>
  <div class="background-bar-overlay">
  </div>
  </div>
  </div>
</template>

<script>
export default {
  name: 'Enter',

}
</script>
<style scoped>
.container {
  width: 100%;
  height: 100%;
  display: grid;
  grid-template-columns: 20% 20% 20% 20% 20%;
  grid-template-rows: 20% 20% 20% 20% 20%;
  position: fixed;
}

.background-bar {
  background-image: url('../../phloxus.jpg');
  grid-area: 1/ 1/ 6/ 6;
  z-index: 0;
  filter: blur(8px);
  -webkit-filter: blur(8px);
}

.background-bar-overlay {
  background-color: #FD60C7;
  grid-area: 1/ 1/ 6/ 6;
  z-index: 1;
  opacity: .2;
}

.flower {
  grid-area: 1/ 2/ 6/ 5;
  background-image: url('../../phloxus.jpg');
  width: 100%;
  height: auto; 
  position: relative;
  z-index: 2;
  border: 3px solid #FE332F;
  margin-top: 5%;
  margin-bottom: 5%;
}

.label {
  grid-area: 2/ 2/ 5/ 5;
  background-color: rgba(0, 0, 0, 0.3);
  z-index: 3;
  margin-left: 10%;
  margin-right: 10%;
  color: white;
  font-family: 'La Belle Aurore', cursive;
  font-weight: bold;
  margin-bottom: 10%;
}

.title {
  font-size: 5.5rem;
  
  text-decoration: underline;
  transition: all 2s;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
    background-image: linear-gradient(to right, #FE2D29, #FE2D29 50%, white 50%);
    background-size: 200% 100%;
    background-position: 100%;
}

.title:hover {
    background-position: 0%;  
  
}

.subtitle {
  font-size: 2.75rem;
  margin-top: -15%;
}
</style>