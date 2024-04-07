<script>
    import '$lib/styles/global.css'
    import Email from "$lib/icons/Email.svelte";
    import Call from "$lib/icons/Call.svelte";
    import Location from "$lib/icons/Location.svelte";
    import Facebook from '$lib/icons/Facebook.svelte';
    import Instagram from '$lib/icons/Instagram.svelte';
    import Twitter from '$lib/icons/Twitter.svelte';
</script>
<!-- Navbar -->
<div class="font-inter font-medium">
    <nav class="px-7 py-2 bg-[#10152ebb] text-white">
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
    <nav class="flex justify-between items-center px-7 py-2 bg-[#10152E] text-white">
        <div class="flex items-center">
            <p><img src="https://upload.wikimedia.org/wikipedia/commons/3/38/Ongole_Medical_College_Logo.png" alt="logo" class="h-12"></p>
            <p class="pl-1 w-32 font-semibold">Abc college of Engineering</p>
        </div>
        <div class="flex" >
            <a href="/" class="px-3 hover:underline">Home</a>
            <a href="/notice" class="px-3 hover:underline">Notice</a>
            <a href="/downloads" class="px-3 hover:underline">Downloads</a>
            <a href="/about" class="px-3 hover:underline">About</a>
            <a href="/contact" class="pl-3 hover:underline">Contact</a>
        </div>
    </nav>
</div>

<slot />
<!-- Footer -->
<div class="flex justify-around px-7 py-5 bg-[#10152E] text-white font-inter font-medium">
    <div class="py-3 basis-1/3">
        <p class="text-2xl">ABC college of Engineering</p>
        <p class="py-2">ABC college of Engineering is one of the finest college of Nepal giving you the world class facilities and services to both the students and teachers as well as parents you know. We provide very friendly environment for students to gain enormous knowledge.</p>
    </div>
    <div class="py-3 basis-1/3">
        <p class="text-xl">Contact Us</p>
        <div class="py-3">
            <ul>
                <li class="flex py-2">
                    <i> <Call /> </i><span class="pl-1">+977-522428</span>
                </li>
                <li class="flex py-2">
                    <i> <Email /> </i><span class="pl-1">abccollege@gmail.com</span>
                </li>
                <li class="flex py-2">
                    <i> <Location /> </i><span class="pl-1">Tulsipur-5, Dang</span>
                </li>
            </ul>
        </div>
        <div class="flex">
            <a href class="px-2"><i > <Facebook/> </i></a>
            <a href class="px-2"><i > <Twitter/> </i></a>
            <a href class="px-2"><i > <Instagram/> </i></a>
        </div>
    </div>
    <div class="py-3 basis-1/4">
        <p class="text-xl">Explore</p>
        <ul class="list-disc py-3 px-4">
            <li class="py-1"><a href class="hover:underline">Home</a></li>
            <li class="py-1"><a href class="hover:underline">Facilities</a></li>
            <li class="py-1"><a href class="hover:underline">Downloads</a></li>
            <li class="py-1"><a href class="hover:underline">Academics</a></li>
            <li class="py-1"><a href class="hover:underline">Security</a></li>
        </ul>
    </div>
</div>
