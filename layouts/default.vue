<template>
  <div>
      <Header class="header"/>
      
      <div class="content-slot">
        <slot />
      </div>
      <Footer class="footer"/>
  </div>
</template>

<style>
html {
  font-family:
    'Heebo',
    Roboto,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  max-width: 100%;
  overflow-x: hidden;
}

</style>
