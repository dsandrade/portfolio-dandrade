<template>
  <div>
    <nuxt />
  </div>
</template>

<style>
html {
  font-family: 'eurostile', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'eurostile', sans-serif;
  font-weight: 800;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.wd-100 {
  width: 100%;
}

/* width */
::-webkit-scrollbar {
  width: 7px;
  border-left: 1px solid #e6ecf8;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #293347;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}

.has-text-weight-normal {
  font-weight: 400 !important;
}

.has-text-primary {
  color: #209cee !important;
}

.has-border-top {
  border-top: 1px solid #e6ecf8;
}

.section.is-primary {
  background-color: #209cee;
  color: #fff;
}

.container.is-narrow {
  max-width: 1200px;
}

.box {
  border-radius: 12px;
}
</style>
