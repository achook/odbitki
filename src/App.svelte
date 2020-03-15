<script>
    import router from 'page'

    // Include our Routes
    import Home from './routes/Home.svelte'

    let page
    const params = {
        name: 'worlds'
    }

    router('/', () => { page = Home })
    router.start()
</script>

<svelte:component this={page} params={params} />