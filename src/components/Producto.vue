<template>
  <div class="producto">
    <div class="card">
      <img class="photo" src="https://source.unsplash.com/1600x900/?coffee">
      <h3 class="title">Producto X</h3>
      <div class="description">
        <p>Breve descripcion del cafe</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Producto"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.producto {
}

.card {
  width: 100%;

  background: white;
  border-radius: 2px;
  box-sizing: border-box;
  box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.1);
  padding: 1rem 0;
  padding-top: 0;
  overflow: hidden;
}

.photo {
  width: 100%;
  display: block;
  margin-bottom: 0.75rem;
}

.title,
.description {
  padding: 0 1rem;
}

.title {
  font-size: 1.75rem;
  margin: 0;
  font-family: "Alegreya Sans", sans-serif;
  color: #333;
  margin-top: 0.5rem;
  font-weight: b700;
}
</style>
