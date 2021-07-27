<template>
  <div class="header">
    <div class="image">
      <img src="@/assets/logo.svg" alt="Hunddle" />
    </div>
    <div class="btn">
      <button>Try It Free</button>
    </div>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 140px;
  max-width: 1140px;
  margin: 0 auto;
}

.btn button {
  width: 250px;
  height: 60px;
  border: 0;
  border-radius: 50px;
  background-color: #fff;
  box-shadow: 2px 2px 2px 2px #ccc;
  font-size: 18px;
  font-weight: 500;
}
</style>
