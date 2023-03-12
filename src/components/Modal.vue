<!-- Do not give standard HTML keyword names to your components
when you use lowercase letters as a compoennet name or start
naming them with capital letters !!! -->

<template>
  <div class="backdrop">
    <div class="modal">
      <h1>Modal Name</h1>
      <p>Modal component</p>
    </div>
  </div>
</template>

<script>
// export default {
//   name: 'Modal',
//   props: {
//     msg: String
//   }
// }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  .modal {
    width: 400px;
    padding:20px;
    margin: 200px auto;
    background: white;
    border-radius: 10px;
  }

  .backdrop {
    top: 0;
    left: 0;
    position: fixed;
    background: rgba(0,0,0,0.5);
    width: 100%;
    height: 100%;
  }

  /* h1 style owerwrite but all h1 tags will be applied unless you use "<style scoped>" above
    In that case styles in this file will be renamed like this: <h1 data-v-xxxxxxxx> ... 
    But this approach should be used in some specific situations not commonly */
  /* h1 {
    color: #3603cf;
    border: none;
    padding: 0;
  } */

  .modal h1 {
    color: #3603cf;
    border: none;
    padding: 0;
  }

  .modal p {
    font-style: normal;
  }
</style>
