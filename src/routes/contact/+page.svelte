<script>
    import Email from "$lib/icons/Email.svelte";
    import Call from "$lib/icons/Call.svelte";
    import Location from "$lib/icons/Location.svelte";
</script>
<main class="flex justify-around font-inter">
    <div class="my-20 ">
        <p class="pb-3 text-2xl font-medium text-[#10152E]">Contact Us</p>
        <div class=" px-3 bg-[#10152eb0] text-white rounded-lg">
            <div class="flex py-3"><i> <Location /> </i><span class="pl-1">Tulsipur-5, Dang</span></div>
            <div class="flex py-3"><i> <Call /> </i><span class="pl-1">+977-522428</span></div>
            <div class="flex py-3"><i> <Email /> </i><span class="pl-1">abccollege@gmail.com</span></div>
        </div>
        <div></div>
    </div>
    <div class="my-20">
        <div class="text-center pb-3 text-2xl font-medium text-[#10152E]">Message/Inquiry</div>
        <div class="border border-[#bebdbd1f] px-8 py-5 shadow-xl">
            <div class="flex">
                <div class="px-5 py-2">
                    <p class="font-mono">First Name</p>
                    <input type="text" name="fname" class="border px-3 py-1 tracking-wide font-mono focus:outline-none">
                </div>
                <div class="px-5 py-2">
                    <p class="font-mono">Last Name</p>
                    <input type="text" name="lname" class="border px-3 py-1 tracking-wide font-mono focus:outline-none">
                </div>
            </div>
            <div class="flex">
                <div class="px-5 py-2">
                    <p class="font-mono">Email</p>
                    <input type="email" name="email" class="border px-3 py-1 tracking-wide font-mono focus:outline-none">
                </div>
                <div class="px-5 py-2">
                    <p class="font-mono">Phone</p>
                    <input type="text" name="phone" class="border px-3 py-1 tracking-wide font-mono focus:outline-none">
                </div>
            </div>
            <div class="px-5 py-2 ">
                <p class="font-mono">Message</p>
                <textarea type="text" name="message" class="border px-3 focus:outline-none w-full h-36 tracking-wide font-mono"></textarea>
            </div>
            <div class=" my-5 mx-5 py-2 text-center bg-[#10152E] font-medium text-white rounded hover:cursor-pointer">Send Message</div>
        </div>
    </div>
</main>