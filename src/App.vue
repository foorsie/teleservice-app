<template>
  <div id="app">
      
      <header class="header-main">
        <Header/>
      </header>

      <TicketSlide/>
      
      <main class="flex-main">
          <Sidebar />
          <Dashboard /> 
      </main>
        
        
    </div>
    

</template>

<script>
import Header from './components/Header.vue'
import Sidebar from './components/Sidebar.vue'
import Dashboard from './components/Dashboard.vue'
import Ticket from './components/Ticket.vue'
import TicketSlide from './components/TicketSlide.vue'


export default {
  name: 'app',
  components: {
    Header,
    Dashboard,
    Sidebar,
    Ticket,
    TicketSlide
  }
}
</script>

<style lang="scss">

*{
  margin:0;
  padding:0;
  box-sizing: border-box;
}

body{
  display: flex;
  flex-direction: column;
  background: #eeefea;
}

html{
  height: 100%;
  min-height: 100%;
  text-rendering: optimizeLegibility;
}

.header-main{
  display: flex;
  flex: 1 0 20%;

}

.flex-main{
  display: flex;
  flex: 1;
  height: 100vh;
}


</style>
