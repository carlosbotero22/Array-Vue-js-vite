<template>
  <h1>{{ name }}</h1>

  <div class="cards m-4" v-for="fruta in arrayFrutas" :key="fruta.id">
    <div class="card" style="width: 18rem">
      <img
        class="card-img-top"
        src="https://comidaa.com/wp-content/uploads/2022/05/Frutas-Con-E-2.jpg"
        alt="Card image cap"
      />
      <div class="card-body">
        <h5 class="card-title">{{ fruta.name }}</h5>
        <p class="card-text">
          {{ fruta.descripcion }}
        </p>
        {{ fruta.precio }}
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>
</template>

<script setup>
const name = 'Vite + Vue';

const arrayFrutas = [
  {
    id: '1',
    name: 'pera',
    precio: '200.000',
    descripcion: 'pera verde',
  },
  {
    id: '2',
    name: 'manzana',
    precio: '200.000',
    descripcion: 'manzana roja',
  },
  {
    id: '3',
    name: 'piña',
    precio: '200.000',
    descripcion: 'piña amarilla',
  },
];
</script>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
