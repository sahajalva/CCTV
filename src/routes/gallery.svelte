<script>
	import Gallery from '../components/Gallery.svelte';
	import { GalleryImages } from '../data/data.js';
	import { each } from 'svelte/internal';
</script>

<section
	class="min-h-screen"
	style="background-image: url('assets/bg.png'); background-size: contain;"
>
	<article class="prose-base lg:prose-xl max-w-7xl mx-auto p-4 text-justify scrollbar-hide">
		<h2 class="text-orange-700">Gallery</h2>

		<!-- <div class="carousel w-full">
			<div id="slide1" class="carousel-item relative w-full">
				<img src="assets/images/img1.jpg" class="w-full" alt="" />
				<div
					class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
				>
					<a href="#slide4" class="btn btn-circle">❮</a>
					<a href="#slide2" class="btn btn-circle">❯</a>
				</div>
			</div>
			<div id="slide2" class="carousel-item relative w-full">
				<img src="assets/images/img2.jpg" class="w-full" alt="" />
				<div
					class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
				>
					<a href="#slide1" class="btn btn-circle">❮</a>
					<a href="#slide3" class="btn btn-circle">❯</a>
				</div>
			</div>
			<div id="slide3" class="carousel-item relative w-full">
				<img src="assets/images/img3.jpg" class="w-full" alt="" />
				<div
					class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
				>
					<a href="#slide2" class="btn btn-circle">❮</a>
					<a href="#slide4" class="btn btn-circle">❯</a>
				</div>
			</div>
			<div id="slide4" class="carousel-item relative w-full">
				<img src="assets/images/img9.jpg" class="w-full" alt="" />
				<div
					class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
				>
					<a href="#slide3" class="btn btn-circle">❮</a>
					<a href="#slide5" class="btn btn-circle">❯</a>
				</div>
			</div>
			<div id="slide5" class="carousel-item relative w-full">
				<img src="assets/images/img8.jpg" class="w-full" alt="" />
				<div
					class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
				>
					<a href="#slide4" class="btn btn-circle">❮</a>
					<a href="#slide6" class="btn btn-circle">❯</a>
				</div>
			</div>
			<div id="slide6" class="carousel-item relative w-full">
				<img src="assets/images/img11.jpg" class="w-full" alt="" />
				<div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
				  <a href="#slide5" class="btn btn-circle">❮</a> 
				  <a href="#slide1" class="btn btn-circle">❯</a>
				</div>
			  </div>
		</div> -->
		<div class="mx-auto">
			<span class="text-black text-lg justify-center"> 
				Use arrow keys to move
			</span>
			<div class="snap-x mx-auto snap-mandatory h-screen flex   overflow-x-scroll scrollbar-hide">
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img1.jpg" alt="" class="mx-auto" />
					<p class="font-bold text-black mx-auto text-center ">
						Inaguration of the Center for Computer Vision Research, 4th February, 2021 by the Chief Guest Dr.
						M.K Panduranga Setty
					</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img8.jpg" alt="" class="mx-auto" />

					<p class="font-bold text-black mx-auto text-center">
						(From right) Dr K N Subramanya, Principal RVCE, Shri Sanjay Sahay Ex-IPS, Shri T
						Shankar, Dr. Ravindra S Kulkarni, HOD Dept of Aerospace, Dr. Ramakanth Kumar P, HOD Dept
						of Computer Science and Dr. M.K. Panduranga Setty, President RSST
					</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img11.jpg" alt="" class="mx-auto " />
					<p class="font-bold text-black mx-auto text-center ">
						Innaguration of Center of CCTV Research
					</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img9.jpg" alt="" class="mx-auto" />
					<p class="font-bold text-black mx-auto text-center">
						Shri Sanjay Sahay lighting the lamp
					</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img2.jpg" alt="" class="mx-auto" />
					<p class="font-bold text-black mx-auto text-center">Lab of Center of CCTV Research</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img4.jpg" alt="" class="mx-auto" />
					<p class="font-bold text-black mx-auto text-center">Lab of Center of CCTV Research</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img5.jpg" alt="" class="mx-auto" />
					<p class="font-bold text-black mx-auto text-center">Activities in CCTV lab</p>
				</div>



				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img13.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img14.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img15.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img16.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img17.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img18.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img19.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img20.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img21.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img22.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img23.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img24.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img25.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img26.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img27.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>				
				<div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/images/img28.jpg" alt="" class="mx-auto" width="50%"/>
					<p class="font-bold text-black mx-auto text-center">Skill Development Program</p>
				</div>



				<!-- <div
					class="snap-start  w-full flex-shrink-0 h-96 mx-auto  justify-center text-2xl scrollbar-hide "
				>
					<img src="assets/photos/CCTV lab Entrance.JPG" alt="" class="mx-auto w-[50%]" />
					<p class="text-bold text-black mx-auto text-center">CCTV research lab</p>
				</div> -->
			</div>
			
		</div>
	</article>
</section>
