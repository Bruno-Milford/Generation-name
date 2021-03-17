<template>
  <div>
    <div id="slogan" class="text-center">
      <h1>Name Gator</h1>
      <br />
      <h6 class="text-secondary">Gerador de nomes utilizando Vue.js, GraphQL, e Node</h6>
    </div>
    <ListName />
  </div>
</template>

<script>
import ListName from './components/ListName'

export default {
  components: { ListName },
  name: 'App'
}
</script>

<style>

#slogan {
  margin-top: 30px;
  margin-bottom: 30px;
}

</style>
