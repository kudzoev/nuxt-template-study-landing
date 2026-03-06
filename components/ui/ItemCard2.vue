<template>
	<div class="arrival__items2">
					<picture>
						<a href="/">
							<source 
								:srcset="`/img/mobile/${bookMobile}.png`" 
								media="(max-width: 805px)">
							<img 
								:src="`/img/dekstop/${bookDesktop}.png`" 
								alt="книга" 
								class="arrival__items2-image"
							>
						</a>
					</picture>
					<p class="arrival__items2-category">
						<a href="/">{{category}}</a>
					</p>
					<p class="arrival__items2-title">
						<a href="/">{{title}}</a> <br>
						<a href="/">{{title2}}</a>
					</p>
					<p class="arrival__items2-author-name">
						<a href="/">{{author}}</a>
					</p>
					<div class="arrival__items2-price">
						<a href="/">{{price}} <b>₽</b></a>
						<p class="arrival__items2-price--strike">1 284₽</p>
						<p class="arrival__items2-price--discont">Выгода 300 ₽</p>
					</div>

					<p class="arrival__items2-rating">
						<span class="arrival__items2-rating-grade">4.9</span>
						<span class="arrival__items2-rating-recommendation">89% рекомендуют</span>
					</p>

					<form class="arrival__items2-bookmark">
						<button class="arrival__items2-cart">
							<p class="arrival__items2-cart-t">В корзину</p>
						</button>
						<button class="arrival__items2-mark">
							<img src="/components/img/dekstop/svg/product-card/bookmark.svg" alt="Закладка">
							<p class="visually-hidden">В корзину</p>
						</button>
					</form>
				</div>
</template>

<script setup>
	defineProps
	(
		{
			bookMobile: 
			{
				type: String,
				required: true
			},
			bookDesktop:
			{
				type: String,
				required: true
			},
			category:
			{
				type: String,
				required: true
			},
			title:
			{
				type: String,
				required: true
			},
			title2:
			{
				type: String,
				required: true
			},
			author:
			{
				type: String,
				required: true
			},
			price:
			{
				type: String,
				required: true
			}
		}
	)
</script>

<style lang="scss" scoped>
	.arrival__items2
	{
	width: 263px;
	background-color: #fff;
	border-radius: var(--border-radius);

	@media(max-width: 805px)
	{
		width: 176px;
		height: 474px;
		padding-bottom: 10px;
		margin-bottom: 9px;
	}

		&-image
		{
			padding-inline: 58px;
			margin-bottom: 15px;
			@media (max-width: 805px)
			{
				padding-left: 111px;
			}
		}
		
		&-category
		{
			margin-left: 20px;
			margin-bottom: 5px;
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
			margin-bottom: 10px;
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
			margin-bottom: 5px;
			font-weight: 700;
			font-size: 18px;
			line-height: 111%;
			color: #fd3a3a;
			transform: translateY(-4px);

			&--strike
			{
				margin-left: 11px;
				position: relative;
				display: inline-block;
				font-weight: 400;
				font-size: 12px;
				line-height: 125%;
				color: rgba(28, 41, 77, 0.5);

				&::before
				{
					content: "";
					border-bottom: 1px solid red;
					position: absolute;
					width: 100%;
					height: 60%;
					transform: rotate(-4deg);
				}
			}
			&--discont
			{
				display: inline-block;
				margin-left: 12px;
				font-weight: 400;
				font-size: 12px;
				color: #0db98c;
			}
		}

		&-rating
		{
			margin-left: 20px;
			margin-bottom: 12px;
			&-grade
			{
				position: relative;
				display: inline-block;
				width: 52px;
				height: 25px;
				font-weight: 500;
				font-size: 12px;
				line-height: 125%;
				text-align: center;
				padding-top: 5px;
				padding-left: 16px;
				color: var(--color-orange);
				background-color: rgba(255, 122, 0, 0.15);
				border-radius: var(--border-radius);
				&::before
				{
					content: '';
					background: url(/public/img/orange-star.svg) no-repeat left;
					position: absolute;
					@include square(20px);
					left: 7px;
					top: 2px;
				}

			}
			&-recommendation
			{
				margin-left: 10px;
				position: relative;
				display: inline-block;
				width: 144px;
				height: 25px;
				font-weight: 500;
				font-size: 12px;
				line-height: 100%;
				color: #7986cb;
				text-align: center;
				padding-top: 7px;
				padding-left: 18px;
				background: rgb(121, 134, 203, 0.15);
				border-radius: var(--border-radius);

				&::before
				{
					content: '';
					background: url(/public/img/thumb.svg) no-repeat left;
					position: absolute;
					@include square(20px);
					left: 9px;
					top: 2px;
				}
			}
		}

		&-bookmark
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
			padding-right: 2px;
			&::before
				{
				position: absolute;
				content: '';
				background: url(/components/img/dekstop/svg/product-card/orange-cart.svg) no-repeat center right;
				@include square(20px);
				left: 24px;
				top: 8px;
				}
			@media (max-width: 805px)
			{
				width: 117px;
				left: 84px;
				top: 8px;
			}

			&-t
			{
				padding-left: 30px;
				font-weight: 500;
				font-size: 14px;
				line-height: 107%;
			}
		}

		&-mark
		{
			padding-bottom: 1px;
			@include square(40px);
			border: var(--border-form);
			border-radius: var(--border-radius);
			display: flex;
			align-items: center;
			justify-content: center;
		}		
	}
</style>



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
			}
		}