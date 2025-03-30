<template>
  <div class="layout">
    <header>header</header>
    <main id='main'>
      <article>article</article>
      <nav>nav</nav>
      <aside>aside</aside>
    </main>
    <footer>footer</footer>
  </div>
</template>

<script>
  export default {
    name: "index"
  }
</script>

<style lang="scss" scoped>
  .layout{
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
  }
  #main {
    flex: 1 0 0;
    /*min-height: 800px;*/
    margin: 0px;
    padding: 0px;
    display: -webkit-flex;
    display: flex;
    -webkit-flex-flow: row;
    flex-flow: row;
  }

  #main > article {
    margin: 4px;
    padding: 5px;
    border: 1px solid #cccc33;
    border-radius: 7pt;
    background: #dddd88;
    -webkit-flex: 3 1 60%;
    flex: 3 1 60%;
    -webkit-order: 2;
    order: 2;
  }

  #main > nav {
    margin: 4px;
    padding: 5px;
    border: 1px solid #8888bb;
    border-radius: 7pt;
    background: #ccccff;
    -webkit-flex: 1 6 20%;
    flex: 1 6 20%;
    -webkit-order: 1;
    order: 1;
  }

  #main > aside {
    margin: 4px;
    padding: 5px;
    border: 1px solid #8888bb;
    border-radius: 7pt;
    background: #ccccff;
    -webkit-flex: 1 6 20%;
    flex: 1 6 20%;
    -webkit-order: 3;
    order: 3;
  }

  header, footer {
    flex: 0 0 auto;
    display: block;
    margin: 4px;
    padding: 5px;
    min-height: 100px;
    border: 1px solid #eebb55;
    border-radius: 7pt;
    background: #ffeebb;
  }
</style>