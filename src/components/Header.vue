<template>
  <div class="container">
    <div class="item border">
      <a href="https://facebook.com/">
        <font-awesome-icon :icon="{prefix:'fab',iconName:'facebook'}" class="icons"/>
      </a>
      <a href="https://instagram.com/">
        <font-awesome-icon :icon="{prefix:'fab',iconName:'instagram'}" class="icons"/>
      </a>
      <a href="https://twitter.com/">
        <font-awesome-icon :icon="{prefix:'fab',iconName:'twitter'}" class="icons"/>
      </a>
    </div>
    <h1 class="item">Amaltea Coffee</h1>
    <!-- <div class="item">right</div> -->
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: {
      type: String
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  display: grid;
  grid-template-columns: 1fr 2fr;
  /* border: 1px solid red; */
  align-items: center;
  justify-items: center;
  margin: 25px 0;
}

.item {
  padding: 0.5rem;
}

.item:nth-child(2) {
  justify-self: start;
}

a {
  color: #2c3e50;
  font-size: 25px;
  margin-right: 10px;
}

a:hover {
  color: rgb(18, 112, 112);
}
h1 {
  margin: 0;
  font-size: 75px;
}

@media (max-width: 1050px) {
  h1 {
    font-size: 45px;
  }
}

@media (max-width: 550px) {
  .container {
    grid-template-columns: 1fr 2fr;
    margin: 1rem 0;
  }

  h1 {
    font-size: 20px;
  }
  a {
    font-size: 20px;
    margin-right: 5px;
  }
}
</style>
