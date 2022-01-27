<template>
<div class="add-card">
   <HeadingComponents mainHeading="add new card" secondaryHeading="new card"/>
   <BaseCard />

   <form @Submit.prevent> 
     <label for="card-number">Card number</label> 
     <input id="card-numnber" type="text" placeholder="XXXX XXXX XXXX XXXX">
     
     <label for="card-name">Cardholder name</label>
     <input id="card-name" type="text" placeholder="Firstname Lastname">    
     
     <div class="month-year">
      <div class="month">
        <label for="Month">Month</label>
        <select name="month" id="month">
          <option value="01">01</option>
          <option value="02">02</option>
          <option value="03">03</option>
          <option value="04">04</option>
          <option value="05">05</option>
          <option value="06">06</option>
          <option value="07">07</option>
          <option value="08">08</option>
          <option value="09">09</option>
          <option value="10">10</option>
          <option value="11">11</option>
          <option value="12">12</option>
          


        </select>
      </div>
     </div>

     <div class="year">
       <label for="year">Year</label>
       <select name="year" id="year">
         <option value="21">21</option>
         <option value="22">22</option>
         <option value="23">23</option>
         <option value="24">24</option>
       </select>

     </div>
     <label for="vendor">Vendor</label>
     <select name="vendor" id="vendor">
       <option value="Bitcoin">Bitcoin Inc</option>
       <option value="Blockchain">Blockchain</option>
       <option value="Evil">Evil Corp</option>
       <option value="Ninja">Ninja Bank</option>

     </select>

     <BaseButton buttonMessage="add card" />
     <BaseButton buttonMessage="back to cards" />
   </form>
</div>

</template>

<script>
import HeadingComponents from "@/components/HeadingComponents.vue";
import BaseCard from "@/components/BaseCard.vue";
import BaseButton from "@/components/BaseButton.vue";
export default {  
  components:{
    HeadingComponents,
    BaseCard,
    BaseButton,
  }

}
</script>

<style>

.add-card{
  display:flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  
  }

.add-card form{
    display: flex;
    flex-direction: column;
    width: 300px;
  }
.month-year{
  display: flex;
}
.month, .year{
  display: flex;
  flex-direction: column;
  width: 48%;

}
</style>