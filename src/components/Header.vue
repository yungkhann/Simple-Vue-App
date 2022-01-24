<template>
  <header class="text-center bg-indigo-500 text-white p-4 mb-10 ">
    <div class="text-3xl md:text-5xl font-bold mb-3  ">
      <i class="fa fa-viruses"></i>
      Covid-19 Tracker Around the World</div>
    <p>API by <a class="text-purple-300" target="_blank" href="https://covid19api.com">covid19api.com</a></p>

  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
