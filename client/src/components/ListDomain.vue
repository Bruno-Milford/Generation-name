<template>
    <div id="main">
        <h5>Dominios <span class="badge badge-info">{{ domains.length }}</span></h5>
        <div class="card">
            <div class="card-body">
                <ul class="list-group">
                <li class="list-group-item" v-for="domain in domains" :key="domain">
                    {{ domain }}
                </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css"
import "font-awesome/css/font-awesome.css"

export default {
  data() {
    return {
        domains: ['AirHub', 'AirStation', 'AirMart', 'JetHub', 'JetStation', 'JetMart', 'FlightHub', 'FlightStation', 'FlightMart']
    }
  }
}
</script>

<style scoped>

#main {
  background-color: #f1f1f1;
  padding-top: 30px;
  padding-bottom: 30px;
}

</style>
