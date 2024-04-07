<script>
    import Left from '$lib/icons/Left.svelte';
    import Right from '$lib/icons/Right.svelte';

    //Carousel
    const carouselPhotos = [
        'https://c1.wallpaperflare.com/preview/968/730/441/building-cheyenne-photos-high-school.jpg',
        'http://hdpsbahu.com/images/Pages/school%20building.jpg',
        'https://thumbs.dreamstime.com/b/middle-school-building-20723831.jpg',
    ]

    let index = 0;
    const next = () =>{
        index = (index + 1) % carouselPhotos.length;
    };
    const previous = () =>{
        // index = (index - 1) % carouselPhotos.length;
        if(index == 0){
            index = carouselPhotos.length - 1;
        }else{
            index = index - 1;
        }
    };

    //News & Events List
    const events = [
        {
            "title": "Happy Father's Day",
            "desc" : "Father's day progra HTML 5, and WordPress. Our education WordPress  themes are super responsive and pre-built demos to help you get started.  Get free Education Bootstrap themes and website templates for building  websites which is also known",
            "date" : "Feb 02",
            "day" : "Wednesday",
        },
        {
            "title": "Happy Father's Day",
            "desc" : "Father's day progra HTML 5, and WordPress. Our education WordPress  themes are super responsive and pre-built demos to help you get started.  Get free Education Bootstrap themes and website templates for building  websites which is also known",
            "date" : "Feb 02",
            "day" : "Wednesday",
        },
        {
            "title": "Happy Father's Day",
            "desc" : "Father's day progra HTML 5, and WordPress. Our education WordPress  themes are super responsive and pre-built demos to help you get started.  Get free Education Bootstrap themes and website templates for building  websites which is also known",
            "date" : "Feb 02",
            "day" : "Wednesday",
        },
    ]


</script>
<main class="font-inter font-medium">
    <!-- Carousel -->
    <!-- Add circular buttons in image to show which one is active -->
    <div class="flex items-center bg-[#10152E]">
        <button class="bg-slate-200 px-1 py-1" on:click={next}><Left /></button>
        <div>
            {#each [carouselPhotos[index]] as src (index)}
                <img {src} alt="" class="h-[400px] w-screen" />
            {/each}
        </div>
        <button class="bg-slate-200 px-1 py-1" on:click={previous}><Right /></button>
    </div>
    <!-- Introduction -->
    <div class="px-7 py-5 bg-[#10152E] border-green border-b-2 border-white-600">
        <div class="text-2xl font-semibold text-white">ABC college of Engineering</div>
        <div class="pt-2 ">
            <p class="w-[250px] float-right pl-5"><img src="https://thumbs.dreamstime.com/b/middle-school-building-20723831.jpg" alt="" class="h-[250px] w-[250px]"></p>
            <p class="w-[680px] text-justify text-white leading-5 font-mono">At ABC College of Engineering, our commitment to excellence in education and student support is unwavering. We strive to provide top-notch facilities and services to nurture the talents and aspirations of our students. Our faculty members are experts in their fields, dedicated to imparting knowledge and fostering critical thinking skills.
                Our state-of-the-art laboratories, libraries, and research centers offer students hands-on experience and access to the latest technologies. We believe in providing a holistic education that prepares students not only for their careers but also for life beyond the classroom. Furthermore, we understand the financial constraints that many students and their families face. </p>
        </div>
    </div>
    <!-- Facilities -->
    <div class="px-7 py-5 bg-[#10152E] border-green border-b-2 border-white-600 text-white">
        <div>
            <p class="text-2xl">Our Facilities</p>
            <div class="flex justify-between py-3 px-2">
                <div>
                    <img src="http://hdpsbahu.com/images/Pages/school%20building.jpg" alt="" class="h-[100px] w-[100px] rounded-full">
                    <p class="pt-2 text-center">Water</p>
                </div>
                <div>
                    <img src="http://hdpsbahu.com/images/Pages/school%20building.jpg" alt="" class="h-[100px] w-[100px] rounded-full">
                    <p class="pt-2 text-center">Water</p>
                </div>
                <div>
                    <img src="http://hdpsbahu.com/images/Pages/school%20building.jpg" alt="" class="h-[100px] w-[100px] rounded-full">
                    <p class="pt-2 text-center">Water</p>
                </div>
                <div>
                    <img src="http://hdpsbahu.com/images/Pages/school%20building.jpg" alt="" class="h-[100px] w-[100px] rounded-full">
                    <p class="pt-2 text-center">Water</p>
                </div>
                <div>
                    <img src="http://hdpsbahu.com/images/Pages/school%20building.jpg" alt="" class="h-[100px] w-[100px] rounded-full">
                    <p class="pt-2 text-center">Water</p>
                </div>
            </div>
        </div>
        <div class="py-3">
            <p>Other Facilities</p>
            <div>
                <ul class="flex flex-wrap py-2 pl-6 list-disc">
                    <li class="basis-1/3 py-1 px-2"> a</li>
                    <li class="basis-1/3 py-1 px-2"> a</li>
                    <li class="basis-1/3 py-1 px-2"> a</li>
                    <li class="basis-1/3 py-1 px-2"> a</li>
                    <li class="basis-1/3 py-1 px-2"> a</li>
                    <li class="basis-1/3 py-1 px-2"> a</li>
                    <li class="basis-1/3 py-1 px-2"> a</li>
                    <li class="basis-1/3 py-1 px-2"> a</li>
                </ul>
            </div>
        </div>
    </div>
    <!-- News & Events -->
    <div class="px-7 py-5 bg-[#10152E] border-green border-b-2 border-white-600 text-white">
        <div>
            <p class="text-2xl">News & Events</p>
        </div>
        <div>
            <ul>
                {#each events as item}
                    <li class="flex bg-[#D9D9D9] h-[88px] my-5">
                        <div class="text-justify px-3 py-1 overflow-hidden ">
                            <p class="text-black text-xl pb-1">{item.title}</p>
                            <p class="text-[#000000b7] text-ellipsis">{item.desc}</p>
                        </div>
                        <div class="flex flex-col items-center justify-center border bg-[#463E3E] text-white">
                            <p class="text-2xl">{item.date}</p>
                            <p class="px-1">{item.day}</p>
                        </div>
                    </li>
                {/each}
            </ul>
        </div>
        <div>
            <p class="w-fit px-3 py-2 mx-auto border hover:cursor-pointer">Load more</p>
        </div>
    </div>

</main>