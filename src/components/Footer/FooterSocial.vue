<template>
    <v-app>
        <v-footer style="height: 40px;" color="rgb(33, 35, 201)" padless>
            <v-row justify="end" align="center">
                <v-btn v-for="(link, index) in socialLinks" :key="index" :href="link.url" target="_blank" icon>
                    <v-icon>{{ link.icon }}</v-icon>
                </v-btn>
                <h1 class="schoolwork">Mais Anima &copy; {{ new Date().getFullYear() }}</h1>
            </v-row>
        </v-footer>
    </v-app>
</template>

<script>
export default {
    data() {
        return {
            socialLinks: [
                { icon: 'mdi-instagram', url: 'https://www.instagram.com/andre_.bernasconi/' },
            ]
        };
    }
};
</script>

<style>
    .schoolwork {
        color: rgb(32, 32, 32);
        text-align: end;
        margin-right: 30px;
        }
</style>