<template>

    <div class="ticket-container">
        <h1>My Tickets</h1>


        <div class="ticket-single">
            <div class="ticket-inner">
                <div class="ticket-tag">
                    <p class="text-small">CIC Ticket</p>    
                </div>
                <div class="ticket-number">
                    <h2>Ticket No 713246</h2>
                    <p class="text-small">Could not contact customer | Customer did not answer so E-Mail sent.</p>
                </div>
                <div class="ticket-assignment">
                    <h5>Reassigned Retailer</h5>
                    <h4>2234 - Autohaus Menlyn</h4>
                </div>
            </div>
            <div class="ticket-info">
               <div class="ticket-inner-container">
                   <div class="row">
                       <ul class="ticket-data-item">
                           <li class="data-single">
                                <h5>VIN Number</h5>
                                <h4>WBA2P320405G28323</h4>
                           </li>
                           <li class="data-single">
                               <h5>Created Date</h5>
                                <h4>2 March 2018</h4>   
                           </li>
                           <li class="data-single">
                               <h5>Date of Closure</h5>
                                <h4>22 March 2018</h4>
                           </li>
                           <li class="data-single">
                               <h5>Actioned by</h5>
                                <h4>John Mcfarlen</h4>
                           </li>
                            <li class="data-single">
                               <h5>Ticket Type</h5>
                                <h4>Battery Guard</h4>
                           </li>
                       </ul>
                   </div>
               </div>
            </div> 
         </div> 

         

         
        </div>

    </div>

</template>


<script>

export default {
    name: 'ticket',
    components: {
    }
}
</script>

<style lang="scss">

   @import '../global.scss';

   

   .ticket-container{
       padding: 20px 0;
   }

   .ticket-single{
       background: $white;
       min-height: 100px;
       position: relative;
       @include box-shadow;
       margin-bottom: 15px;

       .ticket-number{
             margin-top: 2px;

           h2{
            margin-bottom: 3px;
            }
           .text-small{
               @include color($color-secondary);
               @include size(11px);
               @include weight(normal);
           }
       }
       
       .ticket-inner{
           padding: 7px 20px 0 0;

           .ticket-tag{
               background: $color-orange;
               padding: 4px 0 0 7px;
               max-height: 23px;
               @include textcase(uppercase);
           }
       }

       .ticket-info{
           background: $color-grey-lightest;
           height: 45px;
           position: absolute;
           width: 100%;
           bottom :0;
       }

       .ticket-assignment{
           text-align: right;
           margin-top: 2px;

           h4{
               margin-top: 5px;
           }
       }
   }


.ticket-inner {
  display: grid;
  grid-template-columns: 120px 2fr 1fr;
  grid-gap: 35px;
  background-color: #fff;
  color: #444;

  
}

.ticket-inner-container{
      padding-left: 157px;
}



ul.ticket-data-item li{
    display: inline-block;
    list-style-type: none;
    height: 45px;
    padding: 8px 15px 0 15px;
    border-right: 1px solid $color-grey-lighter;
    color: $color-grey-light;

    h5{
        margin-bottom:2px;
    }
}


.ticket-data-item li:nth-child(1){
    padding-left:0;
}

.ticket-data-item li:nth-last-child(1){
    border: none;
}

</style>

