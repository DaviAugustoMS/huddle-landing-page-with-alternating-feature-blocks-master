<template>
  <div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  components: {},
}
</script>

<style>
:root {
  /* Primary */
  --pink: hsl(322, 100%, 66%);
  /* Neutral */
  --very-pale-cyan: hsl(193, 100%, 96%);
  --very-dark-cyan: hsl(192, 100%, 9%);
  --grayish-blue: hsl(208, 11%, 55%);
  --white: #ffffff;
}

html {
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

h1 {
  font-family: 'Poppins';
  font-size: 38px;
  margin-bottom: 20px;
}

button,
a {
  cursor: pointer;
}

span,
p,
a {
  font-family: sans-serif;
}
</style>
