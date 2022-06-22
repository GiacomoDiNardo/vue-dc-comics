<template>
    <div class="container py-3">
        <div class="d-flex justify-content-between align-items-center">
            <div class="header-logo d-flex justify-content-start align-items-center">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <div class="">
                <ul class="d-flex list-unstyled justify-content-end gap-4">
                    <li v-for="(link, i) in headLinks" :key="i">
                        <a class="head-link" :href="link.href">{{ link.name }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TheHeader",
        data() {
            return {
                headLinks: [
                    {
                        name: "Characters",
                        href: "#",
                    },
                    {
                        name: "Comics",
                        href: "#",
                    },
                    {
                        name: "Movies",
                        href: "#",
                    },
                    {
                        name: "TV",
                        href: "#",
                    },
                    {
                        name: "Games",
                        href: "#",
                    },
                    {
                        name: "Collectibles",
                        href: "#",
                    },
                    {
                        name: "Videos",
                        href: "#",
                    },
                    {
                        name: "Fans",
                        href: "#",
                    },
                    {
                        name: "News",
                        href: "#",
                    },
                    {
                        name: "Shop",
                        href: "#",
                    },
                ]
            }
        }
    };
</script>

<style scoped>
    .header-logo img {
        width: 80px;
        height: 80px;
    }

    ul li a {
        color: black;
        text-transform: uppercase;
        text-decoration: none;
        font-size: 14px;
        font-weight: bold;
    }
</style>