<script>
export default {
    props: ["urlImage", "name", "hobbies", "bgColor"]
}
</script>

<template>
    <div :style="{ 'backgroundColor': bgColor, 'fontWeight': 700 }" class="card">
        <div class="card--header">
            <img class="card--image" :src="urlImage" alt="arale">
            <span>{{ name }}</span>
        </div>
        <p> {{ hobbies }} </p>
    </div>
</template>

<style>
.card {
    border: 1px solid black;
}

.card--header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-size: 1.3rem;
    padding: 1rem;
}

.card--image {
    width: 100px;
}
</style>