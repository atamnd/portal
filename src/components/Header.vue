<template>
    <v-app-bar
        app
        color="teal"
        dark
        id="header"
    >
        <router-link to="/">
            <h1 class="ttl">atam's site</h1>
        </router-link>

        <v-spacer></v-spacer>

        <div
            v-for="link in links"
            :key="link"
        >
            <router-link
                :to="link.href"
            >
                <v-btn
                    color="teal lighten-3"
                    class="ml-3"
                >
                    {{link.text}}
                </v-btn>
            </router-link>
        </div>
    </v-app-bar>
</template>

<script>
export default {
    data() {
        return {
            links: [
                {
                    // text: "about",
                    // href: "about"
                },
            ]
        }
    },
}
</script>

<style lang="scss">
a {
    text-decoration: none;
}
.ttl {
    color: #fff;
}
</style>