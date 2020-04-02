<template>
    <footer>Copyright {{getCurrentYear}} <a :href="href">Hello</a></footer>
</template>

<script>
export default {
    data: ()=> ({
        href: 'https://google.co.jp'
    }),
    computed: {
        getCurrentYear() {
            return new Date().getFullYear();
        }
    }
}
</script>

<style>
    footer {
        text-align: center;
        color: blue;
    }
</style>