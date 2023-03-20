<script setup>
    import { ref, onMounted } from 'vue'

  const contador = ref(0)

  function incrementarContador() {
  contador.value++
  }

  function decrementarContador() {
  contador.value--
  }

onMounted(() => {
  console.log(`O valor inicial do contador é ${contador.value}.`)
})


</script>

<template>
  <div>
    <button @click="incrementarContador">Incrementar</button>
    <button @click="decrementarContador">Decrementar</button>
    <p>Valor do contador é: {{ contador }}</p>
  </div>
  <br>
  <div>
    <button @click="incrementarContador">Incrementar</button>
    <button @click="decrementarContador">Decrementar</button>
    <p>Valor do contador é: {{ contador }}</p>
  </div>
</template>

<style scoped>
.info {
  background-color: rgba(35,12,22,1);
  padding: 20px 30px;
  color: rgb(183, 210, 219);
  border-radius: 10px;
}

h1 {
  color: white;
  font-weight: bold;
  font-size: 1.5em;
}

button {
  font-weight: bold;
}

</style>