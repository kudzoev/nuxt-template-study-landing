<template>
	<div class="arrival__items">
					<picture>
						<a href="/">
							<source 
								:srcset="`/img/mobile/${bookMobile}.png`" 
								media="(max-width: 805px)">
							<img 
								:src="`/img/dekstop/${bookDesktop}.png`" 
								alt="книга" 
								class="arrival__items-image"
							>
						</a>
					</picture>
					<p class="arrival__items-category">
						<a href="/">{{category}}</a>
					</p>
					<p class="arrival__items-title">
						<a href="/">{{title}}</a> <br>
						<a href="/">{{title2}}</a>
					</p>
					<p class="arrival__items-author-name">
						<a href="/">{{author}}</a>
					</p>
					<p class="arrival__items-price">
						<a href="/">{{price}} <b>₽</b></a>
					</p>

					<p class="arrival__items-rating">
						<span class="arrival__items-rating-grade" 
						:style="`--star-way: ${starway}; background: ${bcColor}; color: ${Color}; --margin: ${margin}` ">4.9</span>
						<span class="arrival__items-rating-recommendation"
						:style="`--display: ${display}`">89% рекомендуют</span>
					</p>

					<form class="arrival__items-bookmark">
						<button class="arrival__items-cart">
							<p class="arrival__items-cart-t">В корзину</p>
						</button>
						<button class="arrival__items-mark">
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
			},
			starway:
			{
				type: String,
				required: false,
				default: "url(/img/orange-star.svg)"
			},
			bcColor:
			{
				type: String,
				required: true
			},
			Color:
			{
				type: String,
				required: true
			},
			display:
			{
				type: String,
				required: false,
				default: "inline-block"
			},
			margin:
			{
				type: String,
				required: false,
				default: "8px"
			}
		}
	)
</script>

<style lang="scss">
	
	.arrival__items
	{
	--star-way: url(/img/orange-star.svg);
	--display: inline-block;
	--margin: 8px;
	width: 263px;
	background-color: #fff;
	border-radius: var(--border-radius);

	@media(max-width: 805px)
	{
		width: 176px;
		height: 433px;
	}

		&-image
		{
			display: block;
			margin: 0 auto 15px;
			@media (max-width: 805px)
			{	
				width: 126px;
				height: 180px;
				margin-top: -5px;
			}
		}
		
		&-category
		{
			margin-left: 20px;
			margin-bottom: 6px;
			font-weight: 400;
			font-size: 12px;
			line-height: 125%;
			color: rgba(28, 41, 77, 0.5);
			@media (max-width: 805px)
			{
				margin-left: 11px;
				margin-bottom: 6px;
			}
		}

		&-title
		{
			margin-left: 20px;
			margin-bottom: 8px;
			font-weight: 500;
			font-size: 14px;
			line-height: 1.36;
			color: #1c294d;
			display: -webkit-box;
			-webkit-box-orient: vertical;
			-webkit-line-clamp: 3;
			overflow: hidden;
			text-overflow: ellipsis;
			@media (max-width: 805px)
			{
				margin-left: 11px;	
				margin-bottom: 7px;

			}
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
			@media (max-width: 805px)
			{
				padding-left: 10px;
				margin-bottom: 9px;
			}

		}

		&-price
		{
			padding-left: 20px;
			margin-bottom: 8px;
			font-weight: 700;
			font-size: 18px;
			line-height: 111%;
			color: #1c294d;
			transform: translateY(-2px);
			@media (max-width: 805px)
			{
				padding-left: 10px;
				margin-bottom: 3px;
			}
		}

		&-rating
		{
			margin-left: 20px;
			margin-bottom: 12px;
			@media (max-width: 805px)
			{
				margin-left: 10px;
			}
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
				@media (max-width: 805px)
				{
					margin-bottom: var(--margin);	
					background-color: rgb(251, 192, 45, 0.15);
					color: #FBC02D;

				}
				&::before
				{
					content: '';
					background: var(--star-way) no-repeat left;
					position: absolute;
					@include square(20px);
					left: 7px;
					top: 2px;
					@media(max-width:805px)
					{
						background: url(/img/yellow-star.svg) no-repeat left;
					}
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
				@media (max-width: 805px)
				{
					margin-left: 0;
					margin-bottom: -2px;
					display: var(--display);
					width: 144px;
			    	height: 25px;

				}

				&::before
				{
					content: '';
					background: url(/public/img/thumb.svg) no-repeat left;
					position: absolute;
					@include square(20px);
					left: 9px;
					top: 2px;
					@media (max-width: 805px)
					{
						left: 10px;
					}
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
				padding-left: 10px;
				column-gap: 5px;

			
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
				background: url(/components/img/dekstop/svg/product-card/orange-cart.svg) no-repeat center right;
				@include square(20px);
				left: 24px;
				top: 9px;
				@media (max-width: 805px)
				{
					left: 11px;
					top: 7px;
				}
				}
			@media (max-width: 805px)
			{
				width: 117px;
				height: 35px;
			}

			&-t
			{
				padding-left: 30px;
				font-weight: 500;
				font-size: 14px;
				line-height: 100%;
				@media (max-width: 805px)
				{
					padding-left: 23px;
				}
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
			@media(max-width: 805px)
			{
				@include square(35px);
			}
		}		
	}
</style>