<template>
  <div class="home"> 
      <HeadingComponents />
      <BaseCard />
      <a @click="addCard = 'add-card'">
        <BaseButton buttonMessage="Add-card" />
      </a>
  </div>
</template>

<script>
import BaseCard from "@/components/BaseCard.vue";
import HeadingComponents from "@/components/HeadingComponents.vue";
import BaseButton from "@/components/BaseButton.vue";

export default {
  components: {
    BaseCard,
    HeadingComponents,
    BaseButton,
  },

  name: 'App',
  data(){return{
    addCard: 'add-card'
  }}


}

    
</script>

<style>

.home{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items:center;
  padding: 4rem 0;
}

</style>