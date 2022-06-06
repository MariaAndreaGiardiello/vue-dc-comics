<template>
  <main class="main">
        <div class="main-hero"></div>
        <div class="black-container">
            <div class="container">
                <h4 class="main-title">CURRENT SERIES</h4>
                <div class="comics" v-for="i in 12" :key="i"></div>
            </div>
        </div>
        <div class="blue-container">
            <div class="container">
                <nav>
                    <ul>
                        <li>
                            <div><img class="main-icons" src="../assets/img/buy-comics-digital-comics.png" alt=""></div>
                            <div class="icon-text">DIGITAL COMICS</div>
                        </li>
                        <li>
                            <div><img class="main-icons" src="../assets/img/buy-comics-merchandise.png" alt=""></div>
                            <div class="icon-text">DC MERCHANDISE</div>
                        </li>
                        <li>
                            <div><img class="main-icons" src="../assets/img/buy-comics-subscriptions.png" alt=""></div>
                            <div class="icon-text">SUBSCRIPTION</div>
                        </li>
                        <li>
                            <div><img class="main-icons" src="../assets/img/buy-comics-shop-locator.png" alt=""></div>
                            <div class="icon-text">COMIC SHOP LOCATOR</div>
                        </li>
                        <li>
                            <div><img class="main-icons" src="../assets/img/buy-dc-power-visa.svg" alt=""></div>
                            <div class="icon-text">DC POWER VISA</div>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
  </main>
</template>

<script>
export default {
    name: 'MainComponents',
}
</script>

<style lang="scss" scoped>
.main {
    height: 100vh;
    width: 100%;
}
.main-hero {
    background-image: url(../assets/img/jumbotron.jpg);
    height: 300px;
    background-position: fixed;
    background-size: cover;
    background-repeat: no-repeat;
    margin-top: 4px;
}
.black-container {
    background-color: black;
    height: 80px;
    width: 100%;
}
.blue-container {
    background-color: var(--primary-color);
    height: 100px;
    width: 100%;
}

.main-title {
    color: white;
    background-color: var(--primary-color);
    padding: 10px 15px;
    margin-top: -20px;
}
.main-icons {
    height: 35px;
    width: 30px;
    margin: 30px auto;
}

ul {
justify-content: right;
}
li {
display: flex;
margin: 0 25px;
}

.icon-text {
    margin: 43px 10px;
    color: white;
    font-weight: bold;
}
</style>