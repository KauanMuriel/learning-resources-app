<template>
    <button :class="mode">
        <slot></slot>
    </button>
</template>

<script>
export default {
    props: ['mode']
}
</script>

<style scoped>
button {
    padding: 0.75rem 1.5rem;
    background-color: rgb(172, 39, 16);
    border: 1px solid rgb(172, 39, 16);
    border: 0;
    color: white;
    cursor: pointer;
    font-size: 16px;
    font-family: inherit;
}

button:hover, button:active {
    background-color: rgb(143, 33, 14);
    border-color: rgb(143, 33, 14);
}

.flat {
    background-color: transparent;
    color: rgb(172, 39, 16);
}

.flat:hover, .flat:active {
    background-color: transparent;
    color: rgb(143, 33, 14);
}
</style>