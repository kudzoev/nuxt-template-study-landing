<script setup>
	
</script>

<template>
	<div>
		<section class="tg-form--graybc l-tg">
			<div class="container">
				<div class="tg-form">
					<img class="tg-form__logo" src="/components/img/dekstop/svg/searh-line/logo.svg">
					<form class="tg-form__form">
                            <label for="header-search" class="visually-hidden">Search</label>
                            <input class="tg-form__form-input" type="text" id="header-search"
                            placeholder="Введите свой Email и получите скидку">
                            <button class="tg-form__form-input-button" type="submit">
									<img src="./img/dekstop/svg/footer/tg.svg" 
									alt="Значок поиска" 
									class="tg-form__form-input-button-image"
									>
                            </button>
                    </form>
					<ul class="tg-form__soc-media">
						<li class="tg-form__soc-media--fb">
							<picture>
									<source srcset="./img/mobile/svg/footer/fb.svg" 
									media="(max-width: 805px)">
									<img src="./img/dekstop/svg/footer/fb.svg" 
									alt="fb" 
                            </picture>
						</li>
						<li class="tg-form__soc-media--ins">
							<picture>
									<source srcset="./img/mobile/svg/footer/vk.svg" 
									media="(max-width: 805px)">
									<img src="./img/dekstop/svg/footer/inst.svg" 
									alt="ins" 
                            </picture>
						</li>
						<li class="tg-form__soc-media--twt">
							<picture>
									<source srcset="./img/mobile/svg/footer/inst.svg" 
									media="(max-width: 805px)">
									<img src="./img/dekstop/svg/footer/twt.svg" 
									alt="tw" 
                            </picture>
						</li>
					</ul>
				</div>
			</div>
		</section>

		<section class="bg-white line">
			<div class="main-section container l1 ">
				<div class="main-section__buyers">
					<h4 class="main-section__buyers-title">
						Покупателям
					</h4>
					<ul class="main-section__buyers-list hidden-mobile">
						<li class="main-section__buyers-item">Наша почта</li>
						<li class="main-section__buyers-item">Оплата и доставка</li>
						<li class="main-section__buyers-item">Вопросы и ответы</li>
					</ul>
				</div>
				<div class="main-section__izdatel l2">
					<h4 class="main-section__izdatel-title">
						Издательство
					</h4>
					<ul class="main-section__izdatel-list hidden-mobile">
						<li class="main-section__izdatel-item">О компании</li>
						<li class="main-section__izdatel-item">Авторам</li>
						<li class="main-section__izdatel-item">Вакансии</li>
						<li class="main-section__izdatel-item">Контакты</li>
					</ul>
				</div>
				<div class="main-section__books l3">
					<h4 class="main-section__books-title">
						Книги
					</h4>
					<ul class="main-section__books-list hidden-mobile">
						<li class="main-section__books-item">Все категории</li>
						<li class="main-section__books-item">Бестселлеры</li>
						<li class="main-section__books-item">Новинки</li>
						<li class="main-section__books-item">Скидки и акции</li>
					</ul>
				</div>
				<div class="main-section__price">
					<h4 class="main-section__price-title">
						Прайс-лист
					</h4>
					<div class="main-section__price-sign hidden-mobile">
						<img src="/components/img/dekstop/svg/footer/paper.svg
						" alt="img" class="main-section__price-sign-img">
						<p class="main-section__price--download">Скачать прайс-лист</p>
						<p class="main-section__price--size">PDF, 12 Mb</p>
					</div>
				</div>
				<div class="main-section__contacts">
					<h4 class="main-section__contacts-title hidden-mobile">
						Телефон и Email
					</h4>
					<a href="mailto:market@estatut.ru"><p class="main-section__contacts-mail">market@estatut.ru</p></a>
					<a href="tel:89686606550"><p class="main-section__contacts-number">8 (968) 660-65-50</p></a>
				</div>
				<div class="main-section__copyright">
					<p>© 2020 Издательство «Статут»</p>
				</div>
				<div class="main-section__address">
					<p>ул. Лобачевского, 92, корп. 2 119454, г. Москва</p>
				</div>
				<div class="main-section__confid">
					<p>Политика конфиденциальности</p>
				</div>
				<div class="main-section__ofert">
					<p>Договор оферты</p>
				</div>
			</div>
		</section>
	</div>
</template>

<style lang='scss'>
	.tg-form
		{
			display: flex;
			justify-content: space-between;
			height: 90px;
			align-items: center;
			margin-inline: auto;
			border-radius: var(--border-radius);
			@media(max-width:805px)
				{
					height: 165px;
					flex-direction: column;
					justify-content: center;
					column-gap: 24px;
					width: 355px;
					display: grid;
					grid-template-areas: 
					"s	s"
					"b1	b2";
					margin-bottom: 0;
					padding-bottom: 5px;

				}
			&--graybc
			{
				background-color: rgba(40, 47, 54, 0.04);
			}
			&__logo
			{
				position: relative;
				font-weight: 500;
				font-size: 18px;
				line-height: 140%;
				color: #fff;
				@media(max-width:805px)
					{
						grid-area: b1;
					}

			}

			&__form-input
            {

                @include fluid-form-size(393);
                height: var(--input-height); 
                border-radius: var(--border-radius) 0 0 var(--border-radius);
                border: var(--border-form);
                border-right: none;
                padding-left: 14px;
				margin-left: 100px;
				background-color: #fff;
				transform: translateY(-5px);
                &::placeholder
                {
                    color: #1C294D;
                    opacity: 0.5;
					font-weight: 400;
					font-size: 14px;
					line-height: 1.43;
                }
				@media (max-width: 805px)
					{
						width: 220px;
						margin-left: -8px;
						margin-bottom: 5px;
						border-color: transparent;
						grid-area: b2;
						height: 40px;	
					}

                &-button
                {
                    display: inline-flex;
                    align-items: center;
                    justify-content: center;
                    height: 40px;
					margin-top: 7px;
                    min-width: 50px;
                    color: var(--color-white);
                    background-color: var(--color-orange);
                    border-top-right-radius: var(--border-radius);    
                    border-bottom-right-radius: var(--border-radius);  
                    border: none;  
                    column-gap: 6px;
					@media (max-width: 805px)
					{
						border: var(--border-form);
						border-left: none !important;
						border-color: transparent;
					}

                    &-image
                    {
                        @include square(20px);
                        vertical-align: center;
						color: rgba(28, 41, 77, 0.5);
                    }

            }
			}

			&__soc-media
			{
				display: flex;
				column-gap: 15px;
				@media(max-width: 805px)
				{
				grid-area: s;
				justify-content: center;
				align-items: center;
				height: 72px;
				padding-bottom: 6px;
				border-bottom: var(--border-form);
				}
			}


		}

	.main-section
	{
		display: grid;
		grid-template-areas: 
		"b i bk pl ti ."
		"cr cr ad ad con of";
		column-gap: 21px;
		row-gap: 75px;
		padding-bottom: 40px;
		padding-top: 46px;
		@media(max-width:805px)
		{
			grid-template-areas: 
			"b"
			"i"
			"bk"
			"pl"
			"con"
			"of"
			"ti" 
			"ad"
			"cr";

			width: 335px;
			row-gap: 0px;
			margin-left: auto;
			transform: translateX(-10px);
			padding-top: 17px;
			
		
		}
		&__buyers
		{	
			width: 165px;
			grid-area: b;
			@media(max-width: 805px)
			{
				width: 335px;
				height: 60px;
			}

			&-title
			{
				font-weight: 500;
				font-size: 14px;
				line-height: 143%;
				color: #1c294d;
				margin-bottom: 24px;
				@media(max-width: 805px)
				{
					font-weight: 400;
					font-size: 16px;
					line-height: 125%;
					color: #2a3d48;

					&::after
					{
						position: absolute;
						content: '';
						background: url(./img/dekstop/svg/footer/icon.svg) right center no-repeat;
						@include square(20px);
						right: -7px;
					}
				}
			}
			&-list
			{
				font-weight: 400;
				font-size: 14px;
				line-height: 143%;
				color: rgba(40, 47, 54, 0.8);
			}

			&-item
			{
				margin-bottom: 14px;
			}
		}
		&__izdatel
		{
			width: 165px;
			grid-area: i;
			@media(max-width: 805px)
			{
				width: 335px;
				height: 60px;
				
			}
			&-title
			{
				font-weight: 500;
				font-size: 14px;
				line-height: 143%;
				color: #1c294d;
				margin-bottom: 24px;
				@media(max-width: 805px)
				{
					font-weight: 400;
					font-size: 16px;
					line-height: 125%;
					color: #2a3d48;
					&::after
					{
						position: absolute;
						content: '';
						background: url(./img/dekstop/svg/footer/icon.svg) right center no-repeat;
						@include square(20px);
						right: -6px;
					}
				}

			}
			&-list
			{
				font-weight: 400;
				font-size: 14px;
				line-height: 143%;
				color: rgba(40, 47, 54, 0.8);
			}
			&-item
			{
				margin-bottom: 14px;
			}
		}
		&__books
		{
			width: 165px;
			grid-area: bk;
			@media(max-width: 805px)
			{
				width: 335px;
				height: 63px;

			}
			&-title
			{
				font-weight: 500;
				font-size: 14px;
				line-height: 143%;
				color: #1c294d;
				margin-bottom: 24px;
				@media(max-width: 805px)
				{
					font-weight: 400;
					font-size: 16px;
					line-height: 125%;
					color: #2a3d48;
					transform: translateY(2px);
					&::after
					{
						position: absolute;
						content: '';
						background: url(./img/dekstop/svg/footer/icon.svg) right center no-repeat;
						@include square(20px);
						right: 4px;
					}
				}
			}
			&-list
			{
				font-weight: 400;
				font-size: 14px;
				line-height: 143%;
				color: rgba(40, 47, 54, 0.8);
			}
			&-item
			{
				margin-bottom: 14px;
			}
		}
		&__price
		{
			width: 166px;
			grid-area: pl;
			@media(max-width: 805px)
			{
				width: 335px;
				height: 62px;

			}
			&-sign
			{
				display: grid;
				grid-template-areas: 
				"l t"
				"l t2";
				column-gap: 5px;

				&-img
				{
					grid-area: l;
					padding-top: 3px;
				}
			}
			&-title
			{
				font-weight: 500;
				font-size: 14px;
				line-height: 143%;
				color: #1c294d;
				margin-bottom: 24px;
				@media(max-width: 805px)
				{
					font-weight: 400;
					font-size: 16px;
					line-height: 125%;
					color: #2a3d48;
					&::after
					{
						position: absolute;
						content: '';
						background: url(./img/dekstop/svg/footer/icon.svg) right center no-repeat;
						@include square(20px);
						right: -7px;
					}
				}

			}
			&--download
			{
				font-weight: 300;
				font-size: 14px;
				line-height: 143%;
				color: rgba(40, 47, 54, 0.8);
				grid-area: t;

			}

			&--size
			{
				font-weight: 400;
				font-size: 12px;
				line-height: 125%;
				color: rgba(40, 47, 54, 0.5);
				grid-area: t2;
			}
			
		}
		&__contacts
		{
			width: 165px;
			grid-area: ti;
			@media(max-width: 805px)
			{
				width: 335px;
				height: 95px;
				display: flex;
				flex-direction: column-reverse;
				justify-content: space-between;
				transform: translateX(-3px);
				margin-bottom: 25px;
			}

			&-title
			{	
				font-weight: 500;
				font-size: 14px;
				line-height: 143%;
				color: #1c294d;
				margin-bottom: 24px;
			}
			&-mail
			{
				position: relative;
				font-weight: 400;
				font-size: 14px;
				color: rgba(28, 41, 77, 0.8);
				margin-bottom: 14px;
				padding-left: 29px;
				&::before
				{	
					position: absolute;
					content: '';
					background: url(./img/dekstop/svg/footer/1.svg) right center no-repeat;
					@include square(20px);
					left: 5px;
					bottom: 1px;
				}
			}
			&-number
			{
				position: relative;
				font-weight: 400;
				font-size: 14px;
				color: rgba(28, 41, 77, 0.8);
				margin-bottom: 14px;
				padding-left: 29px;
				@media(max-width: 805px)
				{
					padding-left: 28px;
					&::after
					{	
						position: absolute;
						content: '';
						background: url(./img/dekstop/svg/footer/3.svg) right center no-repeat;
						@include square(20px);
						right: 170px;
					}
				}
				&::before
				{	
					position: absolute;
					content: '';
					background: url(./img/dekstop/svg/footer/2.svg) right center no-repeat;
					@include square(20px);
					left: 2px;
					bottom: 1px;
					@media(max-width: 805px)
					{
						bottom: 0px;
						left: 3px;
					}
				}
			}
		}
		&__copyright
		{
			grid-area: cr;
			font-weight: 400;
			font-size: 14px;
			line-height: 143%;
			color: rgba(28, 41, 77, 0.5);
			@media(max-width: 805px)
			{
				width: 335px;
				height: 60px;

			}
		}
		&__address
		{
			grid-area: ad;
			font-weight: 400;
			font-size: 14px;
			line-height: 143%;
			text-align: center;
			color: rgba(28, 41, 77, 0.8);
			padding-right: 16px;
			@media(max-width: 805px)
			{
				width: 335px;
				height: 60px;
				transform: translateX(15px);
				font-weight: 400;
				font-size: 14px;
				padding-top: 2px;
				padding-left: 4px;
				line-height: 143%;
				letter-spacing: -0.01em;
				color: #1c294d;
				margin-bottom: 3px;
				&::before
				{	
					position: absolute;
					content: '';
					background: url(./img/dekstop/svg/footer/pin.svg) right center no-repeat;
					@include square(20px);
					left: -15px;
				}

			}
		}
		&__confid
		{
			grid-area: con;
			font-weight: 400;
			font-size: 14px;
			line-height: 143%;
			text-align: end;
			color: rgba(28, 41, 77, 0.8);
			@media(max-width: 805px)
			{
				width: 335px;
				height: 60px;
				text-align: start;
				opacity: 0.5;

			}
		}
		&__ofert
		{
			grid-area: of;
			font-weight: 400;
			font-size: 14px;
			line-height: 143%;
			text-align: end;
			color: rgba(28, 41, 77, 0.8);
			@media(max-width: 805px)
			{
				width: 335px;
				height: 30px;
				text-align: start;
				transform: translateY(-30px);
				opacity: 0.5;
			}
		}
	}

	.line
	{
		position: relative;
		
		&::after
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 1140px;
				left: 50%;
				transform: translateX(-50%);
				bottom: 27.5%;
				@media(max-width: 805px)
				{
					width: 100%;	
					bottom: 28.3%;

				}
			}
			@media(max-width: 805px)
			{
				&::before
				{
					content: '';
					position: absolute;
					height: 1px;
					background-color: #dfe0e1;
					width: 1140px;
					left: 50%;
					transform: translateX(-50%);
					bottom: 18.7%;
					width: 100%;	
				}
			}
	}

	.l1
	{
		position: relative;
		@media(max-width: 805px)
		{
		&::after
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 100%;
				left: 45%;
				transform: translateX(-42%);
				bottom: 90.7%;
			}
		&::before
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 381px;
				left: 43%;
				transform: translateX(-42%);
				bottom: 61.9%;
			}
		}
	}
	.l2
	{
		@media(max-width: 805px)
		{
		&::after
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 100%;
				left: 45%;
				transform: translateX(-42%);
				bottom: 81.2%;
			}
		&::before
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 381px;
				left: 43%;
				transform: translateX(-42%);
				bottom: 37.9%;
			}
		}
	}
	.l3
	{

		@media(max-width: 805px)
		{
		&::after
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 100%;
				left: 45%;
				transform: translateX(-42%);
				bottom: 71.4%;
			}
		&::before
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 381px;
				left: 43%;
				transform: translateX(-42%);
				bottom: 47.6%;
			}
		}
	}

	





	.l-tg
	{
		position: relative;
		@media(max-width: 805px)
		{
		&::after
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 100%;
				left: 50%;
				transform: translateX(-50%);
				bottom: 0%;
			}
		}
	}


	.bg-white
	{
			background-color: #fff;
	}
	
</style>