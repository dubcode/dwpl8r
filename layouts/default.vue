<template>
  <div>
    <nuxt />
  </div>
</template>

<style lang="scss">
html {
  font-family: 'Montserrat', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
body {
  background: #fff;
}
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
a:focus,
button:focus,
input:focus,
textarea:focus,
:focus {
  outline: none;
}
h1,
h2,
h3,
h4,
h5,
h6,
ul,
li,
p {
  margin: 0;
  padding: 0;
  -webkit-margin-before: 0;
  -webkit-margin-after: 0;
  -webkit-margin-start: 0px;
  -webkit-margin-end: 0px;
  text-align: left;
}
.--row {
  display: block;
  float: left;
  width: 100%;
  max-width: 2560px;
  overflow: hidden;
  position: relative
  ::after {
    content: '';
    display: block;
    clear: both;
  }
}
.--col {
  display: block;
  float: left;
  width: auto;
  overflow: hidden;
  position: relative
  ::after {
    content: '';
    display: block;
    clear: both;
  }
}
.--ctr{
  margin: 0 auto;
  max-width: 1720px;
  padding: 0 2em;
  width: 100%;
}
.--fs{
  height: 100vh;
}
.--flex{
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
}
.app{
  border: 1px solid #ccc;
  border-radius: 10px;
  margin: 2em auto;
  min-height: calc(100vh - 4em);
  width: 500px;
}
</style>
