<template>
  <div class="base-button">
      <button>{{buttonMessage}}</button>
  </div>
</template>

<script>
export default {
    props:[
    'buttonMessage'
    ]
}
</script>

<style>

.base-button button{
    padding: 1rem 2rem;
    text-transform: uppercase;
    margin: 2rem 0;
    cursor: pointer;
    
}

</style>