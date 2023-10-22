<template>
    <section class="p-6 bg-gray-200">
        <header class="flex justify-between">
            <div class="flex items-center">
                <h1 class="font-bold text-lg"><input type="text" value="My App"></h1>
                <p class="text-sm ml-4">
                    Welcome Back, {{ username }}
                </p>
            </div>
            <Nav />
        </header>
    </section>
    <section class="p-6">
        <div class="max-w-3xl mx-auto">
            <iframe style="border-radius:12px"
                src="https://open.spotify.com/embed/episode/2nzGqOnIQAANvJZYzcYLqF?utm_source=generator" width="100%"
                height="152" frameBorder="0" allowfullscreen=""
                allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
            <slot />
        </div>
    </section>
</template>

<script>
import Nav from './Nav.vue'
export default {
    components: { Nav },
    computed: {
        username() {
            return this.$page.props.auth.user.username;
        }
    }
}
</script>
