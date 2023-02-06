<template>
    <li>
        <base-card>
            <header>
                <h3>{{ title }}</h3>
                <base-button mode="flat" @click="deleteResource(id)">Delete</base-button>
            </header>
            <p>{{ description }}</p>
            <nav>
                <a :href="link">View Resource</a>
            </nav>
        </base-card>
    </li>
</template>

<script>
export default {
    props: {
        id: {
            type: String,
            required: true
        },
        title: {
            type: String,
            required: true
        },
        description: {
            type: String,
            required: true
        },
        link: {
            type: String,
            required: true
        }
    },
    inject: ['deleteResource'],
    data() {
        return {

        }
    }
}
</script>

<style scoped>
li {
    margin: auto;
    max-width: 40rem;
    list-style: none;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

a {
    text-decoration: none;
    color: rgb(255, 56, 21);
}

a:hover {
    color: rgb(218, 51, 21);
}
</style>