<template>
  <section id="productos" class="productos">
    <h2>Nuestro Productos</h2>
    <div class="product-grid">
      <Producto/>
      <Producto/>
      <Producto/>
      <Producto/>
    </div>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit.
      Ipsum vero voluptate esse perferendis aperiam deleniti voluptatem dolorum aliquam
      sint dolor reiciendis eos, porro ab molestiae ipsam iste labore officiis! Facere.
    </p>
  </section>
</template>

<script>
import Producto from "./Producto.vue";
export default {
  name: "Productos",
  components: {
    Producto
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.productos {
  background-color: #f5f5f5;
  padding-bottom: 100px;
  padding: 0 5%;
}

.product-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-gap: 15px;
}
h2 {
  margin: 0;
  padding: 50px 0;
}
p {
  padding: 50px;
}

@media (max-width: 1000px) {
  .productos {
    padding: 0;
  }
  .product-grid {
    grid-template-columns: 1fr 1fr;
    padding: 2.5rem;
    grid-gap: 50px;
    margin: 0;
  }
}

@media (max-width: 750px) {
  .product-grid {
    grid-template-columns: 1fr;
    padding: 1rem;
  }
}
</style>
