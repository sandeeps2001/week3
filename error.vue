<script setup>
const error = useError()
const errorhandler = () => {
    navigateTo("/")
}
</script>
<template>
    <div>
        <h1>{{error.statusCode}}</h1>
        <h1>{{ error.statusMessage}}</h1>
        <button @click="errorhandler" class = "rounded mt-7 text-2xl bg-blue-400 px-7 py-4 text-white">go back</button>
    </div>
</template>