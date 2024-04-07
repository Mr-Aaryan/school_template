<script>
    import { Gallery } from "flowbite-svelte";
    import { Carousel, Indicator } from 'flowbite-svelte';
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
  const images1 = [
    {
      alt: 'Gallery',
      src: 'https://excelpublicschool.com/EPS/Content/img/academics/academicsSchedule/2.jpg',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://bournetrust.s3.amazonaws.com/uploads/asset_image/2_291_e.jpg?t=1681806499',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://broxbourne.s3.amazonaws.com/uploads/asset_image/2_13_e.jpg?t=1627639461',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://newageworldschool.com/assets/images/inside-gallery-page/NewAge-world-School-Gallery-Image-1.jpg',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://excelpublicschool.com/EPS/FileUploads/6ac0faef-fba2-4346-9533-32c8908f9fc1@IMG8297.JPG',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://www.jkeducate.co.uk/app/uploads/2022/08/classroom-2093744_1920.jpg.webp',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://content.jdmagicbox.com/comp/mysore/c8/0821px821.x821.090522121743.j1c8/catalogue/excel-public-school-belavadi-mysore-cbse-schools-arfiv.jpg',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://www.excelpublicschool.com/EPS/Content/img/learningBeyond/InnovationLab/6.jpg',
      title: 'gallery'
    },
    {
      alt: 'Gallery',
      src: 'https://5.imimg.com/data5/DJ/PV/GLADMIN-64970456/computer-lab-class.png',
      title: 'gallery'
    },
    
  ];
</script>

<main class="mx-auto py-6">
    <div >
        <Carousel {images} let:Indicators let:Controls on:change={({ detail }) => (image = detail)}>
            <Controls />
            <Indicators />
          </Carousel>
    </div>
    <div class="container mx-auto px-2">
        <h2 class="py-8 text-4xl"><span class="pb-1 border-b border-black">Our Gall</span>ery</h2>
        <div> 
              <Gallery class="gap-4 grid-cols-2 md:grid-cols-3" items={images1} />
        </div>    
    </div>
</main>