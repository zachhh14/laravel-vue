<template>
    <h1 class="text-3xl">Users</h1>


    <div style="margin-top: 600px">
        <p>The current time now is {{ time }}</p>
    </div>
    <Link class="text-blue-500" href="/users" preserve-scroll>Refresh</Link>
</template>

<script>
import Layout from '../Shared/Layout.vue';
import { Link } from '@inertiajs/vue3';

export default {
    layout: Layout,
    props:{
        time: String,
    }
}
</script>


