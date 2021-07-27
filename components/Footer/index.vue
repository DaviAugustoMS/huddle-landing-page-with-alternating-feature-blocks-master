<template>
  <div class="footer">
    <div class="box-footer">
      <span>Ready To Build Your Community</span>
      <Button />
    </div>
    <div class="content-footer">
      <div class="logo">
        <img src="@/assets/logo-footer.svg" alt="Huddle" />
      </div>
      <div class="rest-footer">
        <div class="address">
          <Contact alterText="Location" text="Av. malek assad, N 255" />
          <Contact alterText="Telephone" text="+55 (11) 9 6812-8855" />
          <Contact alterText="Email" text="daviaugusto.developer@gmail.com" />
        </div>
        <div class="faq">
          <nuxt-link to="">About Us</nuxt-link>
          <nuxt-link to="">What We Do</nuxt-link>
          <nuxt-link to="">Faq</nuxt-link>
        </div>
        <div class="faq">
          <nuxt-link to="">Career</nuxt-link>
          <nuxt-link to="">Blog</nuxt-link>
          <nuxt-link to="">Contact Us</nuxt-link>
        </div>
        <div class="icons">
          <nuxt-link to="" class="icon-social">
            <img src="@/assets/facebook.svg" alt="Facebook" />
          </nuxt-link>
          <nuxt-link to="" class="icon-social">
            <img src="@/assets/linkedin.svg" alt="Facebook" />
          </nuxt-link>
          <nuxt-link to="" class="icon-social">
            <img src="@/assets/twitter.svg" alt="Facebook" />
          </nuxt-link>
          <nuxt-link to="" class="icon-social">
            <img src="@/assets/instagram.svg" alt="Facebook" />
          </nuxt-link>
        </div>
      </div>
    </div>
    <div class="copy-right">
      <span>Copyright © 2020 . Todos os direitos reservados.</span>
    </div>
  </div>
</template>
<style scoped>
.footer {
  width: 100%;
  height: 420px;
  background-color: hsl(192, 100%, 9%);
  display: flex;
  flex-direction: column;
  align-items: center;
}

.logo {
  margin-bottom: 40px;
}

.box-footer {
  width: 100%;
  max-width: 600px;
  height: 200px;
  border-radius: 10px;
  background-color: #fff;
  padding: 30px 40px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  position: relative;
  top: -110px;
}

.box-footer span {
  font-size: 22px;
  font-weight: 700;
}
.content-footer {
  width: 100%;
  max-width: 1140px;
  margin: 0 auto;
  margin-top: -50px;
  margin-bottom: 30px;
}

.rest-footer {
  display: flex;
  justify-content: space-between;
}

.rest-footer .faq {
  display: flex;
  flex-direction: column;
}

.rest-footer .faq a {
  color: #fff;
  text-decoration: none;
  font-size: 18px;
  font-weight: 300;
  margin-bottom: 20px;
}

.icons a {
  border: 1px solid #fff;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  display: flex;
  margin-left: 5px;
}

.icons a img {
  margin-left: 6px;
}

.copy-right {
  width: 100%;
  height: 60px;
  max-width: 1140px;
  margin: 0 auto;
  display: flex;
  justify-content: flex-end;
}
.copy-right span {
  color: #fff;
  font-size: 16px;
  font-weight: 500;
}
</style>
