<script>
export default {
  name: 'CarnetElon',
  data() {
    return {
      run: 'RUN 22.222.222-2',
      apellidos: 'MUSK',
      nombres: 'ELON REEVE',
      nacionalidad: 'SUDAFRICANO',
      sexo: 'M',
      fechaNacimiento: '28 JUN 1971',
      numeroDocumento: '222.222.222',
      fechaEmisión: '01 ENE 2025',
      fechaVencimiento: '01 ENE 2030'
    }
  }
}
</script>

<template>
  <div class="carnet">
    <aside>
      <div>
        <span>CEDULA DE IDENTIDAD</span>
        <img width="40" src="../assets/img/chile_bandera.png" alt="Bandera de Chile" />
      </div>
      <img src="../assets/img/foto_elon.jpg" alt="Foto de Elon Musk" />
      <p>{{ run }}</p>
    </aside>

    <main>
      <header>
        <p>REPUBLICA DE CHILE</p>
        <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
      </header>
      <section>
        <article>
          <header>APELLIDOS</header>
          <span>{{ apellidos }}</span>
        </article>
        <article>
          <header>NOMBRES</header>
          <span>{{ nombres }}</span>
        </article>

        <div class="grid-2-columns">
          <article>
            <header>NACIONALIDAD</header>
            <span>{{ nacionalidad }}</span>
          </article>
          <article>
            <header>SEXO</header>
            <span>{{ sexo }}</span>
          </article>
        </div>
        <div class="grid-2-columns">
          <article>
            <header>FECHA DE NACIMIENTO</header>
            <span>{{ fechaNacimiento }}</span>
          </article>
          <article>
            <header>NÚMERO DOCUMENTO</header>
            <span>{{ numeroDocumento }}</span>
          </article>
        </div>
        <div class="grid-2-columns">
          <article>
            <header>FECHA DE EMISIÓN</header>
            <span>{{ fechaEmisión }}</span>
          </article>
          <article>
            <header>FECHA DE VENCIMIENTO</header>
            <span>{{ fechaVencimiento }}</span>
          </article>
        </div>
        <article>
          <header>FIRMA DEL TITULAR</header>
          <span>X Æ A-12</span>
        </article>
      </section>
    </main>
  </div>
</template>

<style scoped>
.carnet {
  width: 400px;
  height: 230px;
  background: #c8deed;
  border-radius: 20px;
  display: grid;
  grid-template-columns: 30% 1fr;
  padding: 15px;
  box-shadow: 0px 0px 10px 2px black;
}

aside div {
  display: flex;
}

aside > img {
  margin-top: 15px;
  width: 100%;
}

aside p {
  text-align: center;
  font-size: 12px;
  font-weight: bold;
}

main {
  padding: 0px 14px;
}

main article {
  margin: 4px 0px;
}

main article header {
  font-weight: bold;
  color: #0235a4;
  font-size: 8px;
}

main header p {
  font-size: 20px;
  margin: 0;
  font-weight: bold;
  color: #0235a4;
}

main header span {
  font-size: 8px;
  color: #399be1;
}

main section {
  margin-top: 10px;
}

main section article span {
  font-size: 13px;
  font-weight: 600;
}

main section .grid-2-columns {
  display: grid;
  grid-template-columns: 50% 50%;
}
</style>
