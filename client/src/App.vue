<template>
  <div>
    <div id="slogan" class="text-center">
      <h1>Name Gator</h1>
      <br />
      <h6 class="text-secondary">Gerador de nomes utilizando Vue.js, GraphQL, e Node</h6>
    </div>
    <ListName />
    <ListDomain />
  </div>
</template>

<script>
import ListName from './components/ListName'
import ListDomain from './components/ListDomain'

export default {
  components: { ListName, ListDomain },
  name: 'App'
}
</script>

<style>

#slogan {
  margin-top: 30px;
  margin-bottom: 30px;
}

</style>
