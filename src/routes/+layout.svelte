<script>
    import '$lib/styles/global.css'
    import Email from "$lib/icons/Email.svelte";
    import Call from "$lib/icons/Call.svelte";
    import Location from "$lib/icons/Location.svelte";
	import Navbar from '$lib/components/Navbar.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<header class="hidden md:block bg-slate-200">
    <nav class="container mx-auto px-6 py-2">
        <div class="flex justify-between align-middle block">
            <div class="flex py-1">
                <p class="flex pr-3">
                    <i><Call /></i>
                    <span class="pl-1">+977-XXXXXX</span>
                </p>
                <p class="flex px-3">
                    <i><Email /></i>
                    <span class="pl-1">abccollege@email.com</span>
                </p>
                <p class="flex px-1">
                    <i><Location /></i>
                    <span class="pl-1">Sankhamul, Kathmandu</span>
                </p>
            </div>
            <a href="#admission" class="bg-yellow-300 px-3 py-1 rounded-3xl">Admission Open</a>
        </div>
    </nav>
</header>

<Navbar />

<slot />

<Footer />
