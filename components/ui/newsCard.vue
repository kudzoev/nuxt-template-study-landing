<template>
	<div class="news__items">
					<picture>
						<a href="/">
							<source 
								:srcset="`/img/mobile/${bookMobile}.png`" 
								media="(max-width: 805px)">
							<img 
								:src="`/img/dekstop/${bookDesktop}.png`" 
								alt="Статья изображение" 
								class="news__items-image"
							>
						</a>
					</picture>
					<p class="news__items-category">
						<a href="/">{{category}}</a>
					</p>
					<p class="news__items-title">
						<a href="/">{{title}}</a> <br>
						<a href="/">{{title2}}</a>
					</p>
					<p class="news__items-main-text">
						<a href="/">{{author}}</a>
					</p>

					<form class="news__items-bookmark">
						<button class="news__items-button">
							<p class="news__items-cart-t">Читать</p>
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
	
	.news__items
	{
	width: 375px;
	background-color: transparent;
	border-radius: var(--border-radius);

	@media(max-width: 805px)
	{
		width: 355px;
		height: 400px;
	}

		&-image
		{
			display: block;
			margin-left: 20px;
			margin-bottom: 15px;
			@media (max-width: 805px)
			{	
				width: 335px;
				height: 210px;
				margin-top: -5px;
				margin-left: 10px;
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
			@media (max-width: 805px)
			{
				margin-left: 11px;
				margin-bottom: 4px;
			}
		}

		&-title
		{
			margin-left: 20px;
			margin-bottom: 9px;
			font-weight: 500;
			font-size: 16px;
			line-height: 125%;
			color: #1c294d;
			@media (max-width: 805px)
			{
				margin-left: 11px;	
				margin-bottom: 8px;

			}
		}

		&-main-text
		{
			padding-left: 20px;
			margin-bottom: 12px;
			letter-spacing: -0.1px;
			opacity: 0.7;
			display: -webkit-box;
			-webkit-box-orient: vertical;
			-webkit-line-clamp: 3;
			overflow: hidden;
			text-overflow: ellipsis;
			font-weight: 400;
			font-size: 14px;
			line-height: 143%;
			color: #1c294d;
			max-width: 335px;
			@media (max-width: 805px)
			{
				padding-left: 10px;
				margin-bottom: 12px;
			}

		}


		&-bookmark
		{
			padding-inline: 20px;
			@media (max-width: 805px)
			{
				padding-inline: 10px;
			}
		}

		&-button
		{
			position: relative;
			width: 180px;
			height: 40px;
			border: var(--border-form);
			border-radius: var(--border-radius);
			text-align: center;
			@media (max-width: 805px)
			{
				width: 335px;
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
	}
</style>