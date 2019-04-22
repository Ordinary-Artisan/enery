<template>
  <div id="app">
    <div class="appContent">
      <router-view/>
    </div>

    <div class="appFooter">
     导航
    </div>
  </div>
</template>

<style>
#app {
  display: flex;
  flex-direction: column;
  height: 100%;
}

.appContent {
  flex: 1;
  overflow-x:hidden;
  overflow-y:auto
}

.appFooter {
  height: 50px;
  border: 1px solid #cac8c8;
  margin-top:7px;
  margin-bottom:1px;

}
</style>

<script>
export default {

}
</script>
