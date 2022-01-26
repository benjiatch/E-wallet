<template>
  <div class="home"> 
      <HeadingComponents />
      <BaseCard />
      <BaseButton buttonMessage="Add card"/>
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
  }


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