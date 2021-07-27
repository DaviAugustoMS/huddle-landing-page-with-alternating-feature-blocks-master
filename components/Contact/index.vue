<template>
  <div>
    <div v-if="alterText === 'Location'" class="icons">
      <img src="@/assets/icon-location.svg" :alt="alterText" />
      <p>{{ text }}</p>
    </div>
    <div v-if="alterText === 'Telephone'" class="icons">
      <img src="@/assets/icon-phone.svg" :alt="alterText" />
      <p>{{ text }}</p>
    </div>
    <div v-if="alterText === 'Email'" class="icons">
      <img src="@/assets/icon-email.svg" :alt="alterText" />
      <p>{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    icon: String,
    alterText: String,
    text: String,
  },
}
</script>

<style>
.icons {
  display: flex;
  margin-bottom: 20px;
}

.icons img {
  width: 16px;
  margin-right: 10px;
}

.icons p {
  color: #fff;
  font-size: 18px;
}
</style>
