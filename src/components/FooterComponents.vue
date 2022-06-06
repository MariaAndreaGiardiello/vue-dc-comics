<template>
  <footer>
      <div class="footer-top">
          <div class="container">
              <div class="footer-text">
              <nav class="column">
                  <div class="link-title">DC COMICS</div>
                  <ul>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                  </ul>
                  <div class="link-title">DC COMICS</div>
                  <ul>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                  </ul>
              </nav>
               <nav class="column">
                  <div class="link-title">DC COMICS</div>
                  <ul>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                  </ul>
              </nav> <nav class="column">
                  <div class="link-title">DC COMICS</div>
                  <ul>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                        <li class="link-list-choice"><a href="">Characters</a></li>
                  </ul>
              </nav>
          </div>
          <div class="footer-logo">
                <img class="logo-big" src="../assets/img/dc-logo-bg.png" alt="">
          </div>
          </div>
      </div>
      <div class="footer-bottom"></div>
  </footer>
</template>

<script>
export default {
    name: 'FooterComponents',
}
</script>

<style lang="scss" scoped>
.footer-top {
    width: 100%;
    height: 250px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    flex-direction: row;
}
.footer-text {
    width: calc(100% / 2);
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
}
a {
    color: gray;
}
li {
    list-style: none;
    font-size: 12px;
}
.column {
    width: calc(100% / 3);
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    text-align: left;
}
.footer-logo {
    width: calc(100% / 2);
}

.logo-big {
    width: 300px;
    height: 300px;
}
</style>