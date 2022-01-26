<template>
    <div class="base-card">

        <article class="chip-logo">
            <img src="@/assets/chip.svg" alt="chip image">
            <img src="@/assets/evil.svg" alt="evil">
        </article>
        
        <article class="number-name-date">

            <section class="number">
                <p>XXXX XXXX XXXX XXXX</p>
            </section>

            <section class="name-date">
                <div class="name">
                     <h6>CARDHOLDER NAME</h6>
                    <p>FIRSTNAME LASTNAME</p>
                </div>
                
                <div class="date">
                    <h6>VALID THRU</h6>
                    <p>MM / YY</p>
                </div>
            </section>
                
        
        </article>



    </div>
  
</template>

<script>
export default {
    data(){
        return{
        }
    }

}
</script>

<style >

.base-card{
    height: 240px;
    width: 380px;
    padding: 1rem;
    border-radius: 0.5rem;
    box-shadow: 0px 0px 12px black;
    color: black;
    z-index: 1;
    text-transform: uppercase;
    background: grey;
    
   
}

.chip-logo{
    height: 95px;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;

}

.chip-logo img:nth-child(2){
    align-self: flex-start;
    opacity: 0.8;
}

.name-date{
    display: flex;
    justify-content: space-between; 
}

.number p{
    height: 37px;
    font-size: 2rem;
    letter-spacing: 1px;
    margin: 0.9rem 0;
}

.date{
    text-align: end;
}

.name h6, .date h6{
    margin-bottom: 5px;
    text-align: left;
}




    

</style>    