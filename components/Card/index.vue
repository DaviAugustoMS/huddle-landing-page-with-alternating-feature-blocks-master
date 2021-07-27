<template>
  <div>
    <div
      class="card"
      v-for="(item, index) in data"
      :key="item.id"
      :style="{ 'flex-direction': index % 2 ? 'row-reverse' : 'row' }"
    >
      <div class="texts">
        <span>{{ item.title }}</span>
        <p>{{ item.text }}</p>
      </div>
      <div class="images" v-if="item.id === 1">
        <img src="@/assets/illustration-grow-together.svg" :alt="item.title" />
      </div>
      <div class="images" v-else-if="item.id === 2">
        <img
          src="@/assets/illustration-flowing-conversation.svg"
          :alt="item.title"
        />
      </div>
      <div class="images" v-else>
        <img src="@/assets/illustration-your-users.svg" :alt="item.title" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({}),
  props: {
    data: Array,
  },
}
</script>
<style>
.card {
  width: 100%;
  max-width: 1140px;
  height: 350px;
  margin: 0 auto;
  border-radius: 10px;
  box-shadow: 2px 2px 2px 2px #ccc;
  margin-bottom: 30px;
  display: flex;
  padding: 20px 0;
  justify-content: space-between;
}
.card .texts {
  width: 50%;
  display: flex;
  justify-content: space-evenly;
  flex-direction: column;

  padding: 40px 70px;
}
.card .texts span {
  font-size: 22px;
  font-weight: 700;
}
.card .images {
  width: 50%;
  display: flex;
  justify-content: flex-end;
  padding-right: 30px;
}

.card .images img {
  height: 100%;
}
</style>
