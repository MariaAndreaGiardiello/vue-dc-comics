<template>
  <main class="main">
        <div class="main-hero"></div>
        <div class="black-container">
            <div class="container">
                <h4 class="main-title">CURRENT SERIES</h4>
                <div class="comics-list">
                    <div class="comics" v-for="(comics , index) in comics" :key="index">
                        <img class="comics-cover" :src="comics.src" alt="">
                        <h5 class="comics-series">{{comics.series}}</h5>
                    </div>
                </div>
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
    data() {
        return{
            comics: [
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        }
    }
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
.comics-list {
    display: flex;
    flex-wrap: wrap;
    height: 100%;
    width: 100%;
}
.comics {
    width: calc(18% - 35px);
    height: 150px;
    background-color: white;
    margin: 25px 10px;
}
.comics-cover {
    height: 150px;
    width: 100%;
}
.comics-series {
    color: white;
    text-transform: uppercase;
    margin: 10px 0;
    font-size: 12px;
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