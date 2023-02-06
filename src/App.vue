<template>
    <the-header title="RememberMe"></the-header>
</template>

<script>
import TheHeader from './components/layouts/TheHeader.vue';

export default {
    components: {
        'the-header': TheHeader
    },
    data() {
        return {
            storedResources: [
                {
                    id: 'official-guide',
                    title: 'Official Guide',
                    description: 'The official Vue.js documentation.',
                    link: 'https://vuejs.org'
                },
                {
                    id: 'google',
                    title: 'Google',
                    description: 'Learn to google.',
                    link: 'https://google.com.br'
                }
            ]
        };
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@400;700&display=swap');

* {
    box-sizing: border-box;
}

html {
    font-family: 'Source Sans Pro', sans-serif;
}

body {
    margin: 0;
}
</style>