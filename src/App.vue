<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
html, body {
  height: 100%;
  width: 100%;
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
#app {
  height: 100%;
  width: 100%;
  font-family: Helvetica Neue, Helvetica, PingFang SC, Hiragino Sans GB, Microsoft YaHei, \\5FAE\8F6F\96C5\9ED1, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
article,
aside,
blockquote,
body, button,
dd,
details,
div,
dl,
dt,
fieldset,
figcaption,
figure,
footer,
form,
h1,
h2,
h3,
h4,
h5,
h6,
header,
hgroup,
hr,
input,
legend,
li,
menu,
nav,
ol,
p,
section,
td,
textarea,
th,
ul {
  margin: 0;
  padding: 0;
}
img {
  border-style: none;
}
a {
  color: #2d8cf0;
  background: 0 0;
  text-decoration: none;
  outline: 0;
  cursor: pointer;
  transition: color .2s ease;
}
/* ::-webkit-scrollbar{
   width: 5px;
   background: #f5f7f9;
} 
::-webkit-scrollbar-thumb{
   -webkit-border-radius: 4px;
   border-radius: 4px;
   background: rgba(0,0,0,0.3);
} */
</style>
