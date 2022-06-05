<template>
  <main class="main">
        <div class="black-container">
            <div class="container">
                <h1 class="main-top-text"> --> content goes here</h1>
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
    height: 180px;
    width: 100%;
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

.main-top-text {
    color: white;
    line-height: 80px;
}
.main-icons {
    height: 35px;
    width: 30px;
    margin: 30px auto;
}

ul {
display: flex;
flex-wrap: wrap;
justify-content: right;
}
li {
list-style: none;
font-size: 12px;
display: flex;
margin: 0 25px;
}

.icon-text {
    margin: 43px 10px;
    color: white;
    font-weight: bold;
}
</style>