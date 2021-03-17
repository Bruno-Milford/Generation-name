<template>
  <div id="main">
      <div class="container">
        <div class="row">
          <div class="col-md">
            <h5>Prefixos <span class="badge badge-info">{{ prefixes.length }}</span></h5>
            <div class="card">
              <div class="card-body">
                <ul class="list-group">
                  <li class="list-group-item" v-for="prefix in prefixes" :key="prefix">
                    {{ prefix }}
                  </li>
                </ul>
                <br />
                <input class="form-control" type="text" placeholder="Digite o prefixo" />
              </div>
            </div>
          </div>
          <div class="col-md">
            <h5>Sufixos <span class="badge badge-info">{{ sufixes.length }}</span></h5>
            <div class="card">
              <div class="card-body">
                <ul class="list-group">
                  <li class="list-group-item" v-for="sufix in sufixes" :key="sufix">
                    {{ sufix }}
                  </li>
                </ul>
                <br />
                <input class="form-control" type="text" placeholder="Digite o sufixo" />
              </div>
            </div>
          </div>
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
      prefixes: ['Air', 'Jet', 'Flight'],
      sufixes: ['Hub', 'Station', 'Mart']
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
