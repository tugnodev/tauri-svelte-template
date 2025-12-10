<script>
    let { children } = $props();
    import "../app.css";
</script>

<main
    class="bg-base-200 w-full h-screen flex flex-col items-center justify-start"
>
    {@render children()}
</main>
