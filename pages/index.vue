<template>
  <div>
    <div class="home">
      <Header />
      <div class="content">
        <div class="texts">
          <h1>Buid The Community Your Fans Will Love</h1>
          <p>
            Huddle re-imagines the way we build communities. You have a voice,
            but so does your audience. Create connections with your users as you
            engage in genuine discussion.
          </p>
          <Button />
        </div>
        <div class="images">
          <img src="@/assets/illustration-mockups.svg" alt="Mockops" />
        </div>
      </div>
    </div>

    <div class="cards">
      <Card :data="showCard" />
    </div>
    <Footer />
  </div>
</template>
<script>
import Header from '@/components/Header'
import textCard from '@/utils/textCard'

export default {
  component: {
    Header,
  },
  data: () => ({
    showCard: [],
  }),
  fetch() {
    this.showCard = textCard
  },
  mounted() {
    console.log(this.showCard)
  },
}
</script>
<style scoped>
.home {
  width: 100%;
  height: 100vh;
  background-color: hsl(193, 100%, 96%);
  background-image: url('@/assets/bg-hero-desktop.svg');
}

.cards {
  width: 100%;
  padding-top: 150px;
  padding-bottom: 300px;
}

.content {
  width: 100%;
  max-width: 1140px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}

.texts {
  width: 50%;
  max-width: 450px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}

.texts p {
  font-size: 18px;
  margin-bottom: 20px;
}

.texts button {
  width: 300px;
  height: 60px;
  font-size: 18px;
  font-weight: 500;
  border: 0;
  border-radius: 50px;
  background-color: hsl(322, 100%, 66%);
  color: #fff;
}

.images {
  width: 50%;
}

.images img {
  width: 100%;
  height: 100%;
}
</style>
