
	<template>
		<div class="container">
			<section class="action">
				<div class="action__slider slider">
					<div class="action__slider-item">
						<div class="slider1">
								<div class="slider-line">
									
									<picture class="slide">
											<source 
												srcset="./img/1111.png" 
												media="(max-width: 805px)">
											<img 
												src="./img/1.png" 
												alt="книга" 
											>
									</picture>
									<picture class="slide">
											<source 
												srcset="./img/222222.png" 
												media="(max-width: 805px)">
											<img 
												src="./img/22.png" 
												alt="книга" 
											>
									</picture>
									<picture class="slide">
											<source 
												srcset="./img/33333.png" 
												media="(max-width: 805px)">
											<img 
												src="./img/33.png" 
												alt="книга" 
											>
									</picture>
									<picture class="slide">
											<source 
												srcset="./img/444444.png" 
												media="(max-width: 805px)">
											<img 
												src="./img/44.png" 
												alt="книга" 
											>
									</picture>



								<!--	<img src="./img/1.png" alt="Первый слайд" class="slide">
									<img src="./img/22.png" alt="Второй слайд" class="slide">
									<img src="./img/44.png" alt="Третий слайд" class="slide">
									<img src="./img/33.png" alt="Третий слайд" class="slide">-->
								</div>
								<button class="btn-prev">
									<img src="./img/left-arrow.svg" alt="Левая кнопка">
								</button>
								<button class="btn-next">
									<img src="./img/left-arrow.svg" alt="Правая кнопка">
								</button>
								<div class="slider-dots"></div>
						</div>
					</div>
				</div>
				<div class="action__daily-book">
					<p class="action__h-time">
						<span class="action__book-day-h">Книга дня</span>
						<span class="action__time-left">08:56:31</span>
					</p>
					<picture>
						<a href="/">
							<source srcset="./img/mobile/png/book-roj.png" 
								media="(max-width: 805px)">
							<img src="./img/dekstop/png/book-roj.png" 
								alt="Самая первая книга" 
								class="action__h-time-image"
							>
						</a>
					</picture>
					<p class="action__book-category">
						<a href="/">Корпоративное право</a>
					</p>
					<p class="action__book-title">
						<a href="/">Инвестирование: способы, риски, субъекты : монография</a>
					</p>
					<p class="action__book-author-name">
						<a href="/">Майфат А.В.</a>
					</p>
					<p class="action__book-price">
						<a href="/">4 450 <b>₽</b></a>
					</p>

					<form class="action__book-cart-bookmark">
						<button class="action__book-cart">
							<p class="action__book-cart--t">В корзину</p>
						</button>
						<button class="action__book-mark">
							<img src="./img/dekstop/svg/product-card/bookmark.svg" alt="Закладка">
							<p class="visually-hidden">В корзину</p>
						</button>
					</form>


				</div>
				<div class="action__banner1">
					<!--<p class="ation__banner1-text">
						Бесплатно доставим <br> ваш заказ при <br> покупке от 2000 ₽
					</p>-->
					<a href="/"> <img src="./img/dekstop/svg/11111.svg" alt="delivery guy">
					</a>
				</div>
				<div class="action__banner2">
					<!--<p class="ation__banner1-text">
						Скидка <br> при регистрации <br> до 15%
					</p>-->
					<a href="/"> <img src="./img/dekstop/svg/22222.svg" alt="chill guy">
					</a>
				</div>
			</section>

			<section class="arrival">
				<div class="arrival__nav">
					<div class="arrival__nav-h">
						<h2 class="arrival__nav-h2">
							Новые поступления
						</h2>
					</div>
					<button class="arrival__nav-btns">
						<a href="/">
							<img src="./img/Dark.svg" alt="buttons">
						</a>
					</button>
				</div>
				<div class="arrival__cards">
					<div class="purple-action">
						<span class="arrival__purple-action-bestseller">Бестселлер</span>
						<span class="arrival__purple-action-present">1+1=3</span>
						<ItemCard
						bookMobile="book-second"
						bookDesktop="book-second"
						category="Корпоративное право"	
						title="Инвестирование: способы,"
						title2="риски, субъекты : монография"
						author="Майфат А.В."
						price="4 450"
						starway="url(/img/yellow-star.svg)"	
						bcColor="rgb(251, 192, 45, 0.15)"
						Color="rgb(251, 192, 45)"
						/>
					</div>	
					<div class="green-action hidden-mobile">
						<span class="arrival__green-action">Новинка</span>
						<ItemCard
						bookMobile="book-children"
						bookDesktop="book-children"
						category="Договорое право"	
						title="Договор коммерческой"
						title2="концессии (франчайзинг). Граж..."
						author="Багдасарян А.Ф."
						price="372"
						/>
					</div>
					<div class="no-action hidden-mobile">
						<span class="arrival__purple-action-bestseller arrival__opacity">Бестселлер</span>
						<ItemCard2
						bookMobile="book-children-second"
						bookDesktop="book-children-second"
						category="Корпоративное право"	
						title="Договор коммерческой"
						title2="концессии (франчайзинг). Граж..."
						author="Башлаков-Николаев И.В."
						price="984"
						/>
					</div>
					<div class="purle-action">
						<span class="arrival__purple-action-bestseller">Бестселлер</span>
						<span class="arrival__purple-action-present">1+1=3</span>
						<ItemCard
						bookMobile="book-second"
						bookDesktop="book-second"
						category="Корпоративное право"	
						title="Инвестирование: способы,"
						title2="риски, субъекты : монография"
						author="Майфат А.В."
						price="450"
						display="none"
						margin="31px"
						/>
					</div>
				</div>
				<div class="arrival__show">
					<p class="arrival__show-text">
						<a href="/">Показать все книги раздела</a>
					</p>
				</div>
			</section>

			<section class="mail-form">
				<h3 class="mail-form__h3">
					Скид<span class="mail-form__h3--decoration">ка 200 ₽ </span>при подписке на рассылку Издательства
				</h3>

				<form class="mail-form__main">
					<label for="mail" class="visually-hidden">ФОРМА ДЛЯ ЭЛЕКТРОННОЙ ПОЧТЫ</label>
					<input type="mail" id="mail" class="mail-form__main-input" placeholder="Введите ваш Email">
					<button class="mail-form__main-button">Подписаться</button>
				</form>
			</section>

			<section class="arrival">
				<div class="arrival__nav">
					<div class="arrival__nav-h">
						<h2 class="arrival__nav-h2">
							Готовятся к выходу
						</h2>
					</div>
					<button class="arrival__nav-btns">
						<a href="/">
							<img src="./img/Dark.svg" alt="buttons">
						</a>
					</button>
				</div>
				<div class="arrival__cards">
					<div class="purple-action">
						<span class="arrival__purple-action-bestseller">Бестселлер</span>
						<span class="arrival__purple-action-present">1+1=3</span>
						<ItemCard
						bookMobile="book-second"
						bookDesktop="book-second"
						category="Корпоративное право"	
						title="Инвестирование: способы,"
						title2="риски, субъекты : монография"
						author="Майфат А.В."
						price="4 450"
						starway="url(/img/yellow-star.svg)"	
						bcColor="rgb(251, 192, 45, 0.15)"
						Color="rgb(251, 192, 45)"
						/>
					</div>	
					<div class="green-action hidden-mobile">
						<span class="arrival__green-action">Новинка</span>
						<ItemCard
						bookMobile="book-children"
						bookDesktop="book-children"
						category="Договорое право"	
						title="Договор коммерческой"
						title2="концессии (франчайзинг). Граж..."
						author="Багдасарян А.Ф."
						price="372"
						/>
					</div>
					<div class="no-action hidden-mobile">
						<span class="arrival__purple-action-bestseller arrival__opacity">Бестселлер</span>
						<ItemCard2
						bookMobile="book-children-second"
						bookDesktop="book-children-second"
						category="Корпоративное право"	
						title="Договор коммерческой"
						title2="концессии (франчайзинг). Граж..."
						author="Башлаков-Николаев И.В."
						price="984"
						/>
					</div>
					<div class="purle-action">
						<span class="arrival__purple-action-bestseller">Бестселлер</span>
						<span class="arrival__purple-action-present">1+1=3</span>
						<ItemCard
						bookMobile="book-second"
						bookDesktop="book-second"
						category="Корпоративное право"	
						title="Инвестирование: способы,"
						title2="риски, субъекты : монография"
						author="Майфат А.В."
						price="450"
						display="none"
						margin="31px"
						/>
					</div>
				</div>
				<div class="arrival__show">
					<p class="arrival__show-text">
						<a href="/">Показать все книги раздела</a>
					</p>
				</div>
			</section>

			<section class="columns">
				<picture>

					<source srcset="./img/mobile/png/columns3.svg" 
					media="(max-width: 805px)">
					<img src="./img/dekstop/png/columns1.png" 
					alt="Колонка первая" 
					class="columns__1">
				</picture>
				<picture>

					<source srcset="./img/mobile/png/columns1.svg" 
					media="(max-width: 805px)">
					<img src="./img/dekstop/png/columns2.png" 
					alt="Колонка вторая" 
					class="columns__2">
				</picture>
				<picture>

					<source srcset="./img/mobile/png/columns2.svg" 
					media="(max-width: 805px)">
					<img src="./img/dekstop/png/columns3.png" 
					alt="Колонка третья" 
					class="columns__3">
				</picture>
				<picture>

					<source srcset="./img/mobile/png/columns3.svg" 
					media="(max-width: 805px)">
					<img src="./img/dekstop/png/columns4.png" 
					alt="Колонка четвертая" 
					class="columns__4">
				</picture>
			</section>
			
			<section class="news">
				<div class="arrival__nav">
					<div class="arrival__nav-h">
						<h2 class="arrival__nav-h2">
							Новости
						</h2>
					</div>
					<button class="arrival__nav-btns">
						<a href="/">
							<img src="./img/Dark.svg" alt="buttons">
						</a>
					</button>
				</div>
				<div class="news__cards">
					<div class="purple-action">
						<newsCard	
						bookMobile="news1"
						bookDesktop="news1	"
						category="16 июня 2020"	
						title="Бесплатный онлайн-семинар. Доктрина "
						title2="stare decisis: борьба за прецедент в рос..."
						author="18 июня в «Клубе цивилистов» пройдет бесплатный онлайн-семинар по проблематике судебного прецедента. Мероприятие приуроч..."
						/>
					</div>	
					<div class="green-action hidden-mobile">
						<newsCard
						bookMobile="news2"
						bookDesktop="new2"
						category="16 июня 2020"	
						title="Бесплатный онлайн-семинар. Доктрина "
						title2="stare decisis: борьба за прецедент в рос..."
						author="18 июня в «Клубе цивилистов» пройдет бесплатный онлайн-семинар по проблематике судебного прецедента. Мероприятие приуроч..."
						/>
					</div>
					<div class="no-action hidden-mobile">
						<newsCard
						bookMobile="news3"
						bookDesktop="news3"
						category="16 июня 2020"	
						title="Бесплатный онлайн-семинар. Доктрина "
						title2="stare decisis: борьба за прецедент в рос..."
						author="18 июня в «Клубе цивилистов» пройдет бесплатный онлайн-семинар по проблематике судебного прецедента. Мероприятие приуроч..."	
						/>
					</div>
				</div>
				<div class="news__show">
					<p class="news__show-text">
						<a href="/">Показать все новости</a>
					</p>
				</div>
			</section>
		</div>
	</template>

	<script setup>
		import ItemCard from './ui/ItemCard.vue'
		import ItemCard2 from './ui/ItemCard2.vue'
		import newsCard from './ui/newsCard.vue'

		import { onMounted} from 'vue'

		onMounted( ()=> {
				const sliderLine = document.querySelector('.slider-line')


				const dotsContainer = document.querySelector('.slider-dots')



				const slides = document.querySelectorAll('.slide')

				slides.forEach((_, index) => {
					const dot = document.createElement('div');
					dot.classList.add('dot')
					if (index === 0) dot.classList.add('active');
					dotsContainer.appendChild(dot);
				}); 

				const dots = document.querySelectorAll('.dot');

				const btnPrev = document.querySelector('.btn-prev')
				const btnNext = document.querySelector('.btn-next')

				let count = 0;

				function init(){
					let width = document.querySelector('.slider1').clientWidth;
					rollSlider(width);
				}

				btnNext.addEventListener('click', function(){
					count++;
					if (count >= slides.length){
						count = 0;
					}
					init();
					updateDots();
				})

				btnPrev.addEventListener('click', function(){
					count--;
					if (count < 0){
						count = slides.length - 1;
					}
					init();
					updateDots();
				})

				function rollSlider(width){
					sliderLine.style.transform = 'translateX(-' + (count * width) +'px)';
				}

				function updateDots(){
					dots.forEach((dot, index) =>{
						if (index === count){
							dot.classList.add('active');
						} else {
							dot.classList.remove('active');
						}
					})
				}

				dots.forEach((dot, index) => {
					dot.addEventListener('click', () => {
						count = index;
						init();
						updateDots();
					})
				})

				function autoPlay(){
					count++;
					if (count >= slides.length) count = 0;
					init();
					updateDots();
				}

				let timer = setInterval(autoPlay, 3000);

				const sliderBlock = document.querySelector('.slider');

				sliderBlock.addEventListener('mouseenter', () => {
					clearInterval(timer);
				})

				sliderBlock.addEventListener('mouseleave', () => {
					timer = setInterval(autoPlay, 3000);
				})

				let xClick = null;

				sliderLine.addEventListener('touchstart', (event) => {
					xClick = event.touches[0].clientX;
				})

				sliderLine.addEventListener('touchend', (event) =>{
					if (!xClick) return;
					let xRelease = event.changedTouches[0].clientX;
					let diff = xClick - xRelease;
					if (diff > 50){
						btnNext.click();
					} else if (diff < -50){
						btnPrev.click();
					}
					xClick = null;
				})
						})

		
	</script>

	<style lang='scss'>
		.action
		{
			margin-bottom: 30px;
			display: grid;
			grid-template-areas: 
			"s	s	db"
			"s	s	db"
			"b1	b2	db";
			gap: 30px;

			@media (max-width: 805px)
			{
				grid-template-areas: 
			"s"
			"db"
			"db"
			"b1"
			"b2";
			gap: 10px;	
			justify-content: center;
			}

			&__slider
			{	
				grid-area: s;
				//background-color: var(--color-lime);
				//width: 750px;
				//height: 360px;
				


				/*&-number
				{
					font-size: 100px;
				}*/
			}

			&__daily-book
			{
				grid-area: db;
				width: 360px;
				background-color: #fff;
				border-radius: var(--border-radius);
				@media(max-width: 805px)
				{
					width: 355px;
					padding-bottom: 10px;
					margin-bottom: 9px;
				}
			}

			&__book
			{
				&-day-h
				{
					font-weight: 500;
					font-size: 16px;
					line-height: 1.25;
				}

				&-category
				{
					margin-left: 20px;
					margin-bottom: 8px;
					font-weight: 400;
					font-size: 12px;
					line-height: 125%;
					color: rgba(28, 41, 77, 0.5);
				}

				&-title
				{
					margin-left: 20px;
					margin-bottom: 8px;
					font-weight: 500;
					font-size: 14px;
					line-height: 1.36;
					color: #1c294d;
				}

				&-author-name
				{
					padding-left: 20px;
					margin-bottom: 8px;
					font-weight: 400;
					font-size: 12px;
					line-height: 1.5;
					letter-spacing: -0.1px;
					color: #1c294d;
					opacity: 0.8;

				}

				&-price
				{
					padding-left: 20px;
					margin-bottom: 10px;
					font-weight: 700;
					font-size: 18px;
					line-height: 111%;
					color: #1c294d;
					transform: translateY(-2px);
				}

				&-cart-bookmark
				{
					padding-inline: 20px;
					display: flex;
					column-gap: 10px;

					@media (max-width: 805px)
					{
						width: 355px;
					}
				}

				&-cart
				{
					position: relative;
					width: 146px;
					height: 40px;
					border: var(--border-form);
					border-radius: var(--border-radius);
					text-align: center;
					&::before
						{
							position: absolute;
							content: '';
							background: url(./img/dekstop/svg/product-card/orange-cart.svg) no-repeat center right;
							@include square(20px);
							left: 24px;
							top: 9px;

							@media (max-width: 805px)
							{
								left: 84px;
								top: 8px;
							}
						}
					@media (max-width: 805px)
					{
						width: 265px;
					}

					&--t
					{
						padding-left: 30px;
						font-weight: 500;
						font-size: 14px;
						line-height: 107%;
					}
				}

				&-mark
				{
					@include square(40px);
					border: var(--border-form);
					border-radius: var(--border-radius);
					display: flex;
					align-items: center;
					justify-content: center;
				}



			}

			&__h-time
			{
				display: flex;
				justify-content: space-between;
				padding: 20px;

				&-image
				{
					padding-inline: 97px;
					margin-bottom: 15px;
					@media (max-width: 805px)
					{
						padding-inline: 111px;
					}
				}
			}

			&__time-left
			{
				padding-top: 5px;
				font-weight: 500;
				font-size: 12px;
				line-height: 1.25;
				text-align: center;
				color: var(--color-orange);
				width: 68px;
				height: 25px;
				background-color: rgba(255, 122, 0, 0.15);
				border-radius: var(--border-radius);
			}

			&__banner1
			{
				grid-area: b1;
				@media(max-width: 805px)
				{
					width: 355px;
				}
			}

			&__banner2
			{
				grid-area: b2;
				@media(max-width: 805px)
				{
					width: 355px;
					margin-bottom: -15px;
				}
			}
		}

		.arrival
		{
			background-color: #fff;
			border-radius: var(--border-radius);
			margin-inline: auto;
			position: relative;
			margin-bottom: 30px;
			@media (max-width: 805px)
			{
				width: 355px;
				margin-bottom: 10px;
			}
			&__nav
			{
				display: flex;
				justify-content: space-between;
				height: 61px;
				border-bottom: var(--border-form);

				&-h
				{
					padding-top: 18px;
					padding-left: 25px;

					@media (max-width: 805px)
					{
						padding-inline: 10px;
					}
				}

				&-h2
				{
					font-weight: 700;
					font-size: 20px;
					line-height: 125%;
					color: #1c294d;
				}
				&-btns
				{
					padding-right: 25px;
					
					@media (max-width: 805px)
					{
						padding-right: 10px;
					}
				}
			}

			&__cards
			{
				display: flex;
				column-gap: 30px;
				padding-bottom: 20px;
				border-bottom: var(--border-form);
				& > *
				{
					position: relative;
				}
				& > *:not(:last-child)::after
				{
					content: '';
					position: absolute;
					right: -15px;
					top: 0px;
					bottom: -20px;
					width: 1px;
					background: #dfe0e1;
					@media (max-width: 805px)
					{
						right: 0px;
					}
				}
					@media (max-width: 805px)
					{
						column-gap: 0px;
					}
					@media (max-width: 1150px)			
					{
						flex-wrap: wrap;
						justify-content: space-evenly;	
					}
			}

			&__show
			{
				height: 40px;
				border-radius: 0 0 5px 5px;
				position: relative;
				&-text
				{	
					padding-block: 10px;
					text-align: center;
					font-weight: 500;
					font-size: 14px;
					line-height: 143%;
					color: #1c294d;
				}
			}

			&__purple-action
			{
				position: relative;
				&-bestseller
				{
					position: relative;
					top: 20px;
					left: 21px;
					display: inline-block;
					width: 86px;
					height: 25px;
					font-weight: 500;
					font-size: 12px;
					line-height: 125%;
					text-align: center;
					padding-top: 5px;
					color: var(--color-purple);
					background-color: var(--color-purple-light);
					border-radius: var(--border-radius);
					@media(max-width: 805px)
					{
						top: 15px;
						left: 11px;
					}
				}

				&-present
				{
					position: relative;
					top: 54px;
					left: -66px;
					display: inline-block;
					width: 54px;
					height: 25px;
					font-weight: 600;
					font-size: 12px;
					line-height: 125%;
					text-align: center;
					padding-top: 5px;
					color: #ff4f52;
					background-color: #FFEEEE;
					border-radius: var(--border-radius);
					@media(max-width: 805px)
					{
						top: 50px;
						left: -75px;
					}
				}
			}

			&__green-action
			{
				
					position: relative;
					top: 20px;
					left: 21px;
					display: inline-block;
					width: 70px;
					height: 25px;
					font-weight: 500;
					font-size: 12px;
					line-height: 125%;
					text-align: center;
					padding-top: 5px;
					color: var(--color-green);
					background-color: #E2F6EC;
					border-radius: var(--border-radius);
				
			}

			&__opacity
			{
				opacity: 0;
			}
		}

		.mail-form
		{
			display: flex;
			justify-content: space-between;
			padding-inline: 45px;
			height: 105px;
			align-items: center;
			margin-inline: auto;
			margin-bottom: 30px;
			background-color: var(--color-blue);
			border-radius: var(--border-radius);
			@media(max-width:805px)
				{
					height: 190px;
					flex-direction: column;
					justify-content: center;
					row-gap: 10px;
					width: 355px;
					margin-bottom: 10px;
				}
			&__h3
			{
				position: relative;
				font-weight: 500;
				font-size: 18px;
				line-height: 140%;
				color: #fff;
				@media(max-width:805px)
					{
						min-width: 335px;
					}
				&--decoration
				{	
					position: relative;
					background: url(./img/VectorOr.svg) no-repeat right;
				}

			}

			&__main
			{
				color: #fff;
				display: flex;
				column-gap: 10px;
				@media(max-width:805px)
				{
					flex-direction: column;
					justify-content: center;
					row-gap: 10px;
				}
				&-input
				{
					height: var(--input-height);
					width: 418px;
					background-color: #fff;
					border-radius: var(--border-radius);
					border: var(--border-form);
					color: rgba(28, 41, 77, 1);
					padding-left: 14px;
					&::placeholder
					{
						font-weight: 400;
						font-size: 14px;
						line-height: 143%;
						color: rgba(28, 41, 77, 0.5);
					}

					@media(max-width: 805px)
					{
						width: 335px;
					}
				}

				&-button
				{
					width: 137px;
					height: var(--input-height);
					border: var(--border-form);
					border-radius: var(--border-radius);
					@media(max-width:805px)
					{
						width: 335px;
					}
				}
			}
		}

		.columns
		{
			display: flex;
			justify-content: space-between;
			margin-bottom: 30px;
			@media(max-width: 805px)
			{
				flex-direction: column;
				align-items: center;
				row-gap: 10px;
				margin-bottom: 10px;
			}
		}

		.news
		{
			background-color: #fff;
			margin-bottom: 30px;
			border-radius: var(--border-radius);
			margin-inline: auto;
			@media (max-width: 805px)
			{
				width: 355px;
				margin-bottom: 20px;
			}
			&__cards
			{
				margin-top: 25px;
				display: flex;
				column-gap: 15px;
				padding-bottom: 25px;
				justify-content: space-around;
				& > *
				{
					position: relative;
				}
				& > *:not(:last-child)::after
				{
					content: '';
					position: absolute;
					right: 0px;
					top: -25px;
					bottom: -25px;
					width: 1px;
					background: #dfe0e1;
					@media (max-width: 805px)
					{
						right: 0px;
						display: none;
					}
				}
					@media (max-width: 805px)
					{
						column-gap: 0px;
					}
					@media (max-width: 1150px)			
					{
						flex-wrap: wrap;
						justify-content: space-evenly;	
					}
			}
			&__show
			{
				height: 40px;
				border-radius: 0 0 5px 5px;
				position: relative;
				border-top: var(--border-form);
				&-text
				{	
					padding-block: 10px;
					text-align: center;
					font-weight: 500;
					font-size: 14px;
					line-height: 143%;
					color: #1c294d;
				}
				@media(min-width: 805px)
				{
					display: none;
				}
			}
		}

		*{
    box-sizing: border-box;
}

.slider1{
    height: 100%;
	width: 100%;
    border: none;
    overflow: hidden;
    position: relative;
	max-width: 100vw;
	@media (max-width: 805px)
			{
				right: 0;
				width: 355px;
			}
	
}

.slider-line{
    display: flex;
    transition: transform 0.6s ease-in-out;
}

.slide{
    width: 100%;
	height: 100%;
    flex-shrink: 0;
    object-fit: cover;
	display: block;
	flex-shrink: 0;
}

.slide img{
	width: 100%;
	display: block;
}

.slider-dots{
    display: flex;
    justify-content: center;
    gap: 5px;
    z-index: 100;
	bottom: 20px;
    position: absolute;
	transform: translateX(-50%);
	left: 50%;
	bottom: 22px;
	
}

.dot {
    width: 25px;
    height: 2px;
    background-color: #fff;
    border-radius: 2px;
    transition: 0.3s;
    opacity: 0.5;

}

.dot.active{
    opacity: 1;
}

.btn-prev{
    background-color: rgba(255, 255, 255, 0.85);
    height: 40px;
    aspect-ratio: 1;
    border-radius: 4px;
    border: none;
	left: 27px;
    top: 44%;
	z-index: 1111;
	position: absolute;
	align-items: center;
	justify-content: center;
	display: flex;
	@media (max-width: 805px)
			{
				display: none;
				
			}
}

.btn-next{
    background-color: rgba(255, 255, 255, 0.85);
    height: 40px;
    aspect-ratio: 1;
    border-radius: 4px;
    border: none;
    top: 44%;
	right: 27px;
	position: absolute;
	display: flex;
	align-items: center;
	justify-content: center;
	@media (max-width: 805px)
			{
				display: none;
			}		
}

.btn-next > img{
	transform: rotate(180deg);
}

	</style>