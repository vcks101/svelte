<script>
  export let pais;
  let p;
  const paises = {
    colombia: [
      "Colombia",
      "Bogota",
      "51,52 millones",
      "peso colombiano",
      "1,142 millones km2",
      "colombia.webp",
    ],
    venezuela: [
      "Venezuela",
      "Caracas",
      "28,2 millones",
      "Bolivar",
      "916.445 km2",
      "venezuela_flag.avif",
    ],
    ecuador: [
      "Ecuador",
      "Quito",
      " 17,8 millones",
      "Dolar estadounidense",
      "256.370 km2",
      "ecuador.jpg",
    ],
    peru: [
      "Peru",
      "Lima",
      "33,72 millones",
      "Sol peruano",
      "1.285.215 km2",
      "peru.jpg",
    ],
    brasil: [
      "Brasil",
      "Brasilia",
      "214,3 millones",
      "Real brasileño",
      "8,51 millones km2",
      "brasil.webp",
    ],
    argentina: [
      "Argentina",
      "Buenos aires",
      "46,23 millones",
      "peso argentino",
      "2.78 millones de km2",
      "argentina.jpg",
    ],
    chile: [
      "Chile",
      "Santiago de chile",
      "19.6 millones",
      "peso chileno",
      "756,626 km2",
      "chile.avif",
    ],
    uruguay: [
      "Uruaguay",
      "Montevideo",
      "3.423 millones",
      "peso uruguayo",
      "176,215 km2",
      "uruguay.png",
    ],
    paraguay: [
      "Paraguay",
      "Asuncion",
      "6.109.644",
      "guarani",
      "406,752 km2",
      "paraguay.png",
    ],
  };
  p = paises[pais];
</script>

<div class="main">
  <div class="col1">
    <img
      src="./src/assets/{p[5]}"
      alt="Bandera_Colombia"
      width="300"
      height="200"
    />
  </div>
  <div class="col2">
    <div class="linea"><strong>Pais:</strong>{p[0]}</div>
    <div class="linea"><strong>Capital:</strong>{p[1]}</div>
    <div class="linea"><strong>Poblacion:</strong>{p[2]}</div>
    <div class="linea"><strong>Moneda:</strong>{p[3]}</div>
    <div class="linea"><strong>Extencion:</strong>{p[4]}</div>
  </div>
</div>

<style>
  .main {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 5px;
    grid-auto-rows: minmax(100px, auto);
    border-radius: 10px;
    border-style: solid;
    border-color: rgb(186, 190, 182);
    border-width: 2px;
    margin: left;
    width: 600px;
    box-shadow: 5px 5px 5px black;
    margin-right: 5px;
    margin-bottom: 10px;
  }

  .col1 {
    grid-column: 1;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
  }

  .col2 {
    grid-column: 2;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
    border-color: black;
    width: max-content;
  }
  strong {
    color: blue;
    font-weight: bolder;
  }

  .linea {
    font-size: 20px;
    margin-bottom: 18px;
  }
</style>
