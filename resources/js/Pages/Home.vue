<template>
    <h1>Hello, {{ name }}</h1>
    <span>In this crash course, we will use the following frameworks:</span>
    <ul>
        <li v-for="framework in frameworks">{{ framework }}</li>
    </ul>

    <nav>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/users">Users</a></li>
            <li><a href="/settings">Settings</a></li>
        </ul>
    </nav>
</template>

<script>
export default {
    props: {
        name: String,
        frameworks: Array,
    }
}
</script>
