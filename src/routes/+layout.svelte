<script>
    import '$lib/styles/global.css'
    import Email from "$lib/icons/Email.svelte";
    import Call from "$lib/icons/Call.svelte";
    import Location from "$lib/icons/Location.svelte";
	import Navbar from '$lib/components/Navbar.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<header class="bg-[#10152ebb]">
    <nav class="container mx-auto px-6 py-2 text-white">
        <div class="flex justify-between align-middle">
            <div class="flex py-1">
                <p class="flex pr-3">
                    <i><Call /></i>
                    <span class="pl-1">+977-522428</span>
                </p>
                <p class="flex px-3">
                    <i><Email /></i>
                    <span class="pl-1">abccollege@gmail.com</span>
                </p>
                <p class="flex px-1">
                    <i><Location /></i>
                    <span class="pl-1">Tulsipur-5, Dang</span>
                </p>
            </div>
            <div class="bg-[#E39621] px-3 py-1 rounded-3xl">Admission Open</div>
        </div>
    </nav>
</header>

<Navbar />

<slot />

<Footer />
