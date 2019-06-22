<template>
  <div class="container">
    <div class="left-container"></div>
    <div class="right-container">
      <h2 class="subtitle">AirNet</h2>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.container {
  position: absolute;
  left: 0;
  top: 0;
  margin: 0 auto;
  height: 100vh;
  display: flex;
  flex-direction: row;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.left-container {
  height: 100vh;
  width: 50vw;
  background: rgb(255, 130, 126);
  background: linear-gradient(
    135deg,
    rgba(255, 130, 126, 1) 0%,
    rgba(255, 90, 95, 1) 30%
  );
  z-index: -10;
}
.right-container {
  position: absolute;
  left: 0;
  top: 0;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: -1;
  padding-right: 1rem;
}

.subtitle {
  font-weight: 300;
  font-size: 6rem;
  font-weight: 800;
  font-family: Montserrat, sans-serif;
  color: #000000;
  word-spacing: 5px;
}

.links {
  padding-top: 15px;
}
</style>
