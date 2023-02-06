<template>
    <li>
        <div>
            <header>
                <h3>{{ title }}</h3>
                <button>Delete</button>
            </header>
        </div>
        <p>{{ description }}</p>
        <nav>
            <a :href="link">View Resource</a>
        </nav>
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
    data() {
        return {

        }
    }
}
</script>

<style scoped>
li {
    margin: auto;
    margin-bottom: 3%;
    max-width: 40rem;
    background-color: rgb(248, 248, 248);
    padding: 1%;
    border-radius: 10px;
    box-shadow: 3px 3px #ccc;
    list-style: none;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

a {
    text-decoration: none;
    color: tomato;
}
</style>