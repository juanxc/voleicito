<template>
  <div class="container">
    <div class="py-5 text-center">
      <h2>Registro de Lugar</h2>
      <p class="lead">
        Registra los datos del lugar donde se juega voley, indicar los datos
        exactos para evitar confusiones :).
      </p>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="form-container">
          <form>
            <div class="form-group">
              <label for="txtNombre">Como se llama?</label>
              <input
                id="txtNombre"
                type="text"
                class="form-control"
                placeholder="Lugar"
              />
            </div>
            <div class="form-group">
              <label for="txtDonde">Donde queda?</label>
              <input
                id="txtDonde"
                type="text"
                class="form-control"
                placeholder="Dirección"
              />
            </div>
            <div class="form-group">
              <label for="sltHoraDesde">A que hora?</label>
              <div class="row">
                <div class="col-md-1"><label>Desde:</label></div>
                <div class="col-md-5">
                  <select id="sltHoraDesde" class="form-control"></select>
                </div>
                <div class="col-md-1"><label>Hasta:</label></div>
                <div class="col-md-5">
                  <select id="sltHoraHasta" class="form-control"></select>
                </div>
              </div>
            </div>
            <div class="row justify-content-center">
              <div class="col-md-4 text-center">
                <button type="submit" class="btn btn-primary btn-block">
                  Guardar
                </button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Registro',
  data() {
    return {
      errors: []
    }
  },
  mounted() {}
}
</script>
