<template>
  <div class="producto">
    <div class="card">
      <img class="photo" src="https://source.unsplash.com/600x400/?coffee,barista,tea">
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
  margin-bottom: 1rem;
}

.title,
.description {
  padding: 0 1rem;
}

.title {
  margin: 0;
  font-family: "Alegreya Sans", sans-serif;
  color: #333;
  margin-top: 1rem;
  font-weight: 700;
}
h3.title {
  margin-top: 1rem;
  font-size: 1.25rem;
}

@media (max-width: 750px) {
  h3.title {
    font-size: 1.25rem;
  }
  .description p {
    margin-top: 0.5rem;
  }
}
</style>
