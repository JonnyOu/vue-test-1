<template>
  <div>
    <Header class="header"/>
    <Body class="body"/>
    <Footer class="footer"/>
  </div>
</template>

<script>
import Header from './header/header.vue';
import Body from './body/body.vue';
import Footer from './footer/footer.vue';

export default {
  name: 'Index',
  props: {
    
  },
  components: {
    Header,
    Body,
    Footer
  }
}
</script>

<style scoped>
  div {
    width: 1000px;
    height: 1500px;
    margin: 10px auto;
  }

  .header {
    height: 5%;
  }
  .body {
    height: 90%;
    margin-top: 20px;
  }
  .footer {
    height: 5%;
  }
</style>
