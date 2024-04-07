<script>
    let isOpen = false;
  
    function toggleMenu() {
      isOpen = !isOpen;
    }
</script>
  
<header class="bg-white border-b">
    <nav class="">
        <div class="container px-6 py-6 mx-auto lg:flex lg:justify-between lg:items-center">
            <div class="flex items-center justify-between">
                <a href="/" class="text-md font-semibold text-blue-500">
                    ABC College
                </a>
  
                  <!-- Mobile menu button -->
                <div class="flex lg:hidden">
                    <button on:click={toggleMenu} type="button" class="text-gray-500 hover:text-gray-600 focus:outline-none focus:text-gray-600" aria-label="toggle menu">
                        {#if !isOpen}
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M4 8h16M4 16h16" />
                        </svg>
                        {:else}
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                        {/if}
                    </button>
                </div>
            </div>
  
              <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
            <div class="{isOpen ? 'translate-x-0 opacity-100' : 'opacity-0 -translate-x-full'} absolute inset-x-0 z-20 w-full px-6 py-4 transition-all duration-300 ease-in-out bg-white shadow-md lg:bg-transparent lg:shadow-none lg:mt-0 lg:p-0 lg:top-0 lg:relative lg:w-auto lg:opacity-100 lg:translate-x-0 lg:flex lg:items-center">
            <ul class="flex flex-col space-y-8 lg:flex-row lg:items-center lg:space-y-0 lg:-px-8">
                <li><a class="block font-medium lg:mx-8 hover:underline" href="/">Home</a></li>
                <li><a class="block font-medium lg:mx-8 hover:underline" href="/about">About</a></li>
                <li><a class="block font-medium lg:mx-8 hover:underline" href="/gallery">Gallery</a></li>
                <li><a class="block font-medium lg:mx-8 hover:underline" href="/contact">Contact</a></li>
                <li><a class="block font-medium lg:mx-8 hover:underline" href="/notice">Notices</a></li>
                <li><a class="block font-medium lg:mx-8 hover:underline" href="/downloads">Downloads</a></li>
            </ul>
          </div>
      </div>
  </nav>
</header>
  