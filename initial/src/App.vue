

<template>
  <div class="parent-page">
      <!-- <second-page class="block"/> -->
      <first-page class="block"/>
  </div>
</template>


<script>
  import FirstPage from './components/FirstPage.vue'
  // import SecondPage from './components/SecondPage.vue'
  export default {
      // components: { FirstPage, SecondPage }
      // components: { SecondPage }
      components: { FirstPage }
  }
</script>


<style>
  .parent-page {
      width: 100%;
      height: 100%;
      position: fixed;
      top: 0;
      left: 0;
      display: flex;
      align-items: center;
      align-content: center;
      justify-content: center;
      overflow: auto;
      /* background-color: #F5F5F5; */
  }
  .block {
      display: block;
  }

</style>