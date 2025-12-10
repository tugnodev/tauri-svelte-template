<script lang="ts">
    import { cn } from "$lib/cn";
    import { invoke } from "@tauri-apps/api/core";
    import {
        Navbar,
        NavBrand,
        NavLi,
        NavUl,
        NavHamburger,
        P,
        ImagePlaceholder,
    } from "flowbite-svelte";
</script>

<main class="w-full max-w-8xl h-full flex flex-col">
    <Navbar class="">
        <NavBrand href="/">
            <img
                src="/svelte.svg"
                class="me-3 h-6 sm:h-9"
                alt="Flowbite Logo"
            />
            <span class="self-center text-xl font-semibold whitespace-nowrap"
                >Flowbite</span
            >
        </NavBrand>
        <NavHamburger />
        <NavUl>
            <NavLi class="" href="/">Home</NavLi>
            <NavLi class="" href="/about">About</NavLi>
            <NavLi class="" href="/docs/components/navbar">Navbar</NavLi>
            <NavLi class="" href="/pricing">Pricing</NavLi>
            <NavLi class="" href="/contact">Contact</NavLi>
        </NavUl>
    </Navbar>

    <div class="flex flex-col p-4 gap-6">
        <ImagePlaceholder size="sm" />
        <ImagePlaceholder imgOnly />
        <ImagePlaceholder size="md" />
        <ImagePlaceholder size="lg" />
    </div>
</main>
