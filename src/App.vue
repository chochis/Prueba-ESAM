<template>
  <div class="container">
    <header class="header">
      <h1>PRUEBA TECNICA ESAM</h1>
    </header>

    <div class="main-content">
      <h2>Menú Principal</h2>
      <div class="button-group">
        <BotonComponente title="Perfil Personal" iconClass="mdi-account-box-outline" />
        <BotonComponente title="Registro de Programas" iconClass="mdi-text-box-plus-outline" />
        <BotonComponente title="Docentes" iconClass="mdi-account-search-outline" />
        <BotonComponente title="Postulantes" iconClass="mdi-account-question-outline" />
        <BotonComponente title="Programas" iconClass="mdi-text-box-outline" />
        <BotonComponente title="Certificaciones Docentes" iconClass="mdi-certificate-outline" />
      </div>
    </div>

    <footer class="footer">
      <p>&copy; 2024 Sistema Académico. Todos los derechos reservados.</p>
    </footer>
  </div>
</template>

<script>
import BotonComponente from './components/BotonComponente.vue';

export default {
  components: {
    BotonComponente
  }
}
</script>

<style>
/* --- Estilos Generales --- */
body, html {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  text-align: center;
}

.header, .footer {
  background-color: #003366;
  color: white;
  padding: 20px;
  text-align: center;
}

.main-content {
  flex: 1;
  padding: 20px;
}
.button-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.button-group > * {
  flex: 0 1 calc(33.333% - 20px);
  margin: 15px;
}
</style>