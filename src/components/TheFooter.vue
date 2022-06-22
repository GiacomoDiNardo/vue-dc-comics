<template>
    <div class="footer-bg">
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-5 py-5">
                    <ul class="d-flex flex-wrap list-unstyled gap-5">
                        <li class="m-height">
                            <h3>DC Comics</h3>
                            <ul class="list-unstyled">
                                <li v-for="link in DcComicsLinks" :key="link">
                                    <a href="#">{{ link }}</a>
                                </li>
                            </ul>
                        </li>
                        <li class="m-height">
                            <h3>DC</h3>
                            <ul class="list-unstyled">
                                <li v-for="link in DcLinks" :key="link">
                                    <a href="#">{{ link }}</a>
                                </li>
                            </ul>
                        </li>
                        <li class="m-height">
                            <h3>Sites</h3>
                            <ul class="list-unstyled">
                                <li v-for="link in sitesLinks" :key="link">
                                    <a href="#">{{ link }}</a>
                                </li>
                            </ul>
                        </li>
                        <li class="m-height">
                            <h3>Shop</h3>
                            <ul class="list-unstyled">
                                <li v-for="link in shopLinks" :key="link">
                                    <a href="#">{{ link }}</a>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </div>
                <div class="col-6 footer-logo">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TheFooter",
        data () {
            return {
                DcComicsLinks : [
                     "Characters",
                     "Comics",
                     "Movies",
                     "TV",
                     "Games",
                     "Video",
                     "News",
                ],     
                DcLinks : [
                    "Terms Of Use",
                    "Privacy policy (New)",
                    "Ad Choices",
                    "Advertising",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact Us",
                ],
                sitesLinks : [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa",
                ],
                shopLinks : [
                    "Shop DC",
                    "Shop DC Collectibles",
                ],
            }
        }
    };
</script>

<style>
.footer-bg {
    background-image: url("../../public/img/footer-bg.jpg");
    background-size: cover;
    color: white;
    font-size: 12px;
}

ul li h3 {
    text-transform: uppercase;
    font-size: 18px;
    font-weight: bold;
}

ul li a {
    display: inline-block;
    text-decoration: none;
    color: grey;
    margin-bottom: 3px;
}

.m-height {
    max-height: 150px;
}

.footer-logo {
    height: 400px;
    display: flex;
    align-items: center;
    overflow: hidden;
}
</style>