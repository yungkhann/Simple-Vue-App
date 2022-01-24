<template>
  <select
      @change="onChange()"
      v-model="selected" class="form-select mt-10 block w-full border  border-indigo-600 p-3 rounded outline-none">

    <option :value="country.ID" v-for="country in countries">{{country.Country}}</option>
  </select>

</template>

<script>
export default {
  name: "CountrySelect",
  props:['countries'],
  data(){
    return{
      selected:0
    }
  },
  methods:{
    onChange(){
      const country = this.countries.find((i) => i.ID === this.selected)
      this.$emit('get-country',country)
    }
  }
}
</script>

<style scoped>

</style>