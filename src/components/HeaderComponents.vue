<template>
  <header class="header">
      <div class="container">
          <div class="header-logo">
          <img class="logo" src="../assets/img/dc-logo.png" alt=""/>
        </div>
        <nav class="header-nav">
          <ul>
            <li>CHARACTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLECTIBLES</li>
            <li>VIDEOS</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
          </ul>
        </nav>
      </div>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponents',
}
</script>

<style lang="scss" scoped>
.header {
  height: 80px;
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
}
  .header-logo {
    width: 20%;
    text-align: center;
  }
    .logo {
    width: 50px;
    height: 50px;
    margin-top: 15px;
  }

  .header-nav {
    width: 80%;
  }
  ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: right;
    line-height: 80px;
  }
  li {
    list-style: none;
    font-size: 12px;
    margin: 0 10px;
  }

  li:hover {
    border-bottom: 1px solid;
    border-color: var(--primary-color);
  }
</style>