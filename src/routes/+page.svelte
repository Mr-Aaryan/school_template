<script>
    import { Carousel, Indicator } from 'flowbite-svelte';
	import Cards from '../lib/components/Cards.svelte';

    let image;
    const images = [
        {
      alt: 'School Building',
      src: 'https://c1.wallpaperflare.com/preview/968/730/441/building-cheyenne-photos-high-school.jpg',
      title: 'School Building'
    },
    {
      alt: 'School Building',
      src: 'https://i0.wp.com/avenuemail.in/wp-content/uploads/2021/09/3-1.jpg?fit=1600%2C1067&ssl=1',
      title: 'school building'
    },
    {
      alt: 'School Building',
      src: 'https://www.jkeducate.co.uk/app/uploads/2022/08/classroom-2093744_1920.jpg.webp',
      title: 'School Building'
    },
    {
      alt: 'School Building',
      src: 'https://www.ejable.com/wp-content/uploads/2023/11/Japanese-school-students-2.webp',
      title: 'School Building'
    },
    {
      alt: 'School Building',
      src: 'https://3.files.edl.io/4cef/23/04/24/180648-a08aced7-5823-4211-b842-8af7338b55d2.jpg',
      title: 'school building'
    },
    {
      alt: 'School Building',
      src: 'https://kmcschool.edu.np/wp-content/uploads/2024/03/kmc-banner-school1-scaled.jpg',
      title: 'School Building'
    },

  ];

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
            "title": "Father's Day",
            "desc" : "Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident ab nulla quod dignissimos vel non corrupti doloribus voluptatum eveniet",
            "date" : "Feb 02",
            "day" : "Wednesday",
        },
        {
            "title": "Teachers Day",
            "desc" : "Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident ab nulla quod dignissimos vel non corrupti doloribus voluptatum eveniet",
            "date" : "Feb 02",
            "day" : "Wednesday",
        },
        {
            "title": "Sports Day",
            "desc" : "Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident ab nulla quod dignissimos vel non corrupti doloribus voluptatum eveniet",
            "date" : "Feb 02",
            "day" : "Wednesday",
        },
    ]


</script>
<main class="font-inter font-medium">
    <!-- Carousel -->
    <div>
        <Carousel {images} let:Indicators let:Controls on:change={({ detail }) => (image = detail)}>
            <Controls />
            <Indicators />
          </Carousel>
    </div>
    <!-- Introduction -->
    <div class="container mx-auto py-16 px-3">
        <h2 class="text-center text-5xl font-bold">Introduction</h2>
        <p class="mt-10 max-w-5xl mx-auto text-center text-lg">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
    
    <Cards />

    <div class="container mx-auto px-5 py-2 lg:px-32 lg:pt-24">
        <div class="-m-1 flex flex-wrap md:-m-2">
          <div class="flex w-1/2 flex-wrap">
            <div class="w-1/2 p-1 md:p-2">
              <img
                alt="gallery"
                class="block h-full w-full rounded-lg object-cover object-center"
                src="https://assets-global.website-files.com/65de4c6f8dc17dc010f8ac55/65de4e8fa9dea47849bfe182_654d5b61a2e2c9c8d6cdeae7_5f57c46384cca65e79589acf_students1.jpeg" />
            </div>
            <div class="w-1/2 p-1 md:p-2">
              <img
                alt="gallery"
                class="block h-full w-full rounded-lg object-cover object-center"
                src="https://static-cse.canva.com/blob/1256366/studyingtips1.jpg" />
            </div>
            <div class="w-full p-1 md:p-2">
              <img
                alt="gallery"
                class="block h-full w-full rounded-lg object-cover object-center"
                src="https://assets-api.kathmandupost.com/thumb.php?src=https://assets-cdn.kathmandupost.com/uploads/source/news/2023/opinion/DownPostFilePhoto1-1698683987.jpg&w=900&height=601" />
            </div>
          </div>
          <div class="flex w-1/2 flex-wrap">
            <div class="w-full p-1 md:p-2">
              <img
                alt="gallery"
                class="block h-full w-full rounded-lg object-cover object-center"
                src="https://collegecountdown.scholarshare529.com/wp-content/uploads/2020/10/Smiling_AdobeStock_35308534.jpeg" />
            </div>
            <div class="w-1/2 p-1 md:p-2">
              <img
                alt="gallery"
                class="block h-full w-full rounded-lg object-cover object-center"
                src="https://www.thoughtco.com/thmb/hILwwgdLhyr1VITjTTm9kEOUIDM=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/startingcollege-58d177633df78c3c4ff303ba.jpg" />
            </div>
            <div class="w-1/2 p-1 md:p-2">
              <img
                alt="gallery"
                class="block h-full w-full rounded-lg object-cover object-center"
                src="https://images.ctfassets.net/gogvzi849aaj/432s68B1VAyLuZ0WBCNEFx/35fd9ba545167966487b4268e476e073/2_women_studying_with_books_and_laptop_at_university.jpg?fm=webp&q=50" />
            </div>
          </div>
        </div>
      </div>
    
    <!-- News & Events -->
    <div class="container mx-auto px-6 py-10">
        <h2 class="text-center text-2xl font-semibold">News & Events</h2>
        <div>
            <ul>
                {#each events as item}
                    <li class="flex border rounded mt-5 px-3 py-2">
                        <div class="flex flex-col items-center px-1 py-2 rounded bg-[#463E3E] text-white">
                            <p class="text-2xl">{item.date}</p>
                            <p class="px-1">{item.day}</p>
                        </div>
                        <div class="text-justify px-3 py-1">
                            <h3 class="text-black text-xl pb-1">{item.title}</h3>
                            <p class="text-[#000000b7] text-ellipsis">{item.desc}</p>
                        </div>
                    </li>
                {/each}
            </ul>
        </div>
        <div class="w-fit mt-10 mx-auto">
            <a href="/notice" class="w-24 rounded px-3 py-2 border hover:cursor-pointer">Load more</a>
        </div>
    </div>

</main>

<section class="bg-white dark:bg-gray-900">
    <div class="container px-6 py-10 mx-auto">
        <div class="lg:-mx-6 lg:flex lg:items-center">
            <img class="object-cover object-center lg:w-1/2 lg:mx-6 w-full h-96 rounded-lg lg:h-[36rem]" src="https://t3.ftcdn.net/jpg/03/25/99/70/360_F_325997011_wCC5Rjt8Lltt2Vat6IZJLmAvhpiBHYd3.jpg" alt="">

            <div class="mt-8 lg:w-1/2 lg:px-6 lg:mt-0">
                <p class="text-5xl font-semibold text-blue-500 ">“</p>

                <h1 class="text-2xl font-semibold text-gray-800 dark:text-white lg:text-3xl lg:w-96">
                    Changing the education system
                </h1>

                <p class="max-w-lg mt-6 text-gray-500 dark:text-gray-400 ">
                    “ Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore quibusdam ducimus libero ad
                    tempora doloribus expedita laborum saepe voluptas perferendis delectus assumenda rerum, culpa
                    aperiam dolorum, obcaecati corrupti aspernatur a. ”
                </p>

                <h3 class="mt-6 text-lg font-medium text-blue-500">Mia Brown</h3>
                <p class="text-gray-600 dark:text-gray-300">Principal at ABC College</p>
            </div>
        </div>
    </div>
</section>