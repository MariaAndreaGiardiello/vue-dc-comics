<template>
  <header class="header">
      <div class="container">
          <div class="header-logo">
            <img class="logo" src="../assets/img/dc-logo.png" alt=""/>
          </div>
          <nav class="header-nav">
            <ul>
              <li v-for="(link, index) in links" :key="index" :class="{active : link.current}"><a :href="link.url">{{link.text}}</a></li>
            </ul>
          </nav>
      </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponents',
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false,
        },
        {
          text: "COMICS",
          url: "#",
          current: true,
        },
        {
          text: "MOVIES",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "GAMES",
          url: "#",
          current: false,
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false,
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false,
        },
        {
          text: "FANS",
          url: "#",
          current: false,
        },
        {
          text: "NEWS",
          url: "#",
          current: false,
        },
        {
          text: "SHOP",
          url: "#",
          current: false,
        },
      ]
    }
  }
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
    justify-content: right;
    line-height: 80px;
  }
  li {
    font-size: 12px;
    margin: 0 10px;
  }
  a {
    color: black;
  }
  li:hover {
    border-bottom: 4px solid;
    border-color: var(--primary-color);
  }
  a:hover {
    color: var(--primary-color);
  }
</style>