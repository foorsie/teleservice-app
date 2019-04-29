<template>
    <header class="flex-header">
        <div class="row">
          <div class="logo-brand">
            <figure><img src="../assets/bmw-group-vector-logo.svg" alt=""> </figure>
          </div>
        </div>
    </header>
</template>

<script>
export default {
  name: 'header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">

.flex-header{
  background: #fff;
  box-shadow: 1px 1px 8px #e2e2e2;
  padding: 0em 01em;
  display: flex;
  flex: 1;
  z-index: 8888;
}

.logo-brand {
    width: 75px;
}

</style>
