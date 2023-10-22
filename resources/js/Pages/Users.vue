<template>
    <Layout>
        <h1 class="text-3xl">Users</h1>
    </Layout>


    <div style="margin-top: 500px">
        <p>The current time now is {{ time }}</p>
    </div>
</template>

<script>
import Layout from '../Shared/Layout.vue'

export default {
    components: { Layout },
}
</script>


