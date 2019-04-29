<template>

    <div class="dashboard-wrapper">

        <h1>Dashboard</h1>
        <div class="grid-container">
            <div class="grid">
                <div class="item">
                    <h2>My Performance</h2>
                </div>
                <div class="item">
                    <h2>My Assigned Tickets</h2>
                </div>
                <div class="item">
                    <h2>Callback Tickets</h2>
                </div>
            </div>
            <div class="grid-2">
                <div class="item">
                    <h2>Total TIP Tickets</h2>  
                </div>
                <div class="item">
                    <h2>Tickets closed this month</h2>
                </div>
                <div class="item">
                    <h2>Time per ticket</h2>
                </div>
                <div class="item">
                    <h2>Time per ticket</h2>
                </div>
            </div>
        </div>
        <Ticket/>
    </div>

</template>


<script>
import Ticket from './Ticket.vue'

export default {
    name: 'dashboard',
    components: {
        Ticket,
    }
}
</script>

<style lang="scss">

   @import '../global.scss';

  .main{
      background: rgb(247, 247, 247);
      display: flex;
      flex:auto;
  }

  .dashboard-wrapper {
    width: 100%;
    padding: 2em;
    }

  .grid-container{
      width: 100%;
  }

 .grid {
  display: grid;
    grid-template-columns: 3fr 1fr 1fr;
    grid-template-rows: 300px;
    grid-gap: 20px;
    margin-bottom: 20px;
}

 .grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr; /* doesn't work as expected */
  grid-template-rows: 150px;
  grid-gap: 20px;
  margin-bottom: 20px;
}

.item {
    background-color: #fff;
    box-shadow: 2px 3px 6px rgba(0, 0, 0, 0.1);
    padding: 1em;
}



</style>

