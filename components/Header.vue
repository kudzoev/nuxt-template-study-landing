<template>
	<div class="white-bc">
	<header class="header container">
            <div class="header__contact-info">
                <nav class="header__delivery">
                    <ul class="header__delivery-list">
                        <li class="header__delivery-link">
                            <a href="/" 
                            class="sign-map">
                            Москва
                            </a>
                        </li>
                        <li class="header__delivery-link">
                            <a href="/" 
                            class="sign-box">
                            Доставка и оплата
                            </a>
                        </li>
                        <li class="header__delivery-link">
                            <a href="/" 
                            class="sign-default">
                            Адрес и часы работы
                            </a>
                        </li>
                    </ul>
                </nav>
                <div class="header__contacts">
                    <ul class="header__contact-info-list">
                        <li class="contact-info__email">
                            <a href="mailto:market@estatut.ru" class="email">
                                market@estatut.ru
                            </a>
                        </li>
                        <li class="contact-info__link">
                            <a href="tel:89686606550" class="number__header number">
                                8 (968) 660-65-50
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="header__search-menu">
                <div class="search-menu"> 
                    <div class="search-menu__logo-form">
                        <a href="/" class="big-logo-link">
                            <picture>
                                <source srcset="./img/mobile/svg/search/logo.svg" 
                                media="(max-width: 805px)">
                                <img src="./img/dekstop/svg/searh-line/logo.svg" 
                                alt="Статут" 
                                class="big-logo"
                                >
                            </picture>
                        </a>
                        <form class="header__form">
                            <label for="header-search" class="visually-hidden">Search</label>
                            <input class="header__form-input" type="text" id="header-search"
                            placeholder="Автор, название, ISBN">
                            <button class="header__form-input-button" type="submit">
                                <!--<img src="/img/mobile/svg/search/lupa.svg" alt="Значок поиска" 
                                class="header__form-input-button-image">-->
								<picture>
									<source srcset="./img/mobile/svg/search/lupa.svg" 
									media="(max-width: 805px)">
									<img src="./img/dekstop/svg/searh-line/lupa.svg" 
									alt="Значок поиска" 
									class="header__form-input-button-image"
									>
                            	</picture>
                                <span class="header__form-input-button--mobile ">Искать</span>
                            </button>
                        </form>
                    </div>
					<nav>
						<ul class="header__catalog header__catalog--order">
							<li class="header__catalog-item catalog-sign">
								<a href="/">
									<img 
									src="./img/dekstop/svg/searh-line/burger.svg" 
									alt="Значок меню" width="20" height="20">
								</a>
							</li>
							<li class="header__catalog-item hidden-mobile">
								<a href="/">
									Каталог
								</a>
							</li>
							<li class="header__catalog-item hidden-mobile">
								<a href="/">
									Авторы
								</a>
							</li>
							<li class="header__catalog-item hidden-mobile">
								<a href="/">
									Новинки
								</a>
							</li>
							<li class="header__catalog-item hidden-mobile">
								<a href="/" class="header__catalog-item--red">
									Скидки
								</a>
							</li>
							<li class="header__catalog-item hidden-mobile">
								<a href="/">
									Партнёрам
								</a>
							</li>
							<li class="header__catalog-item hidden-mobile">
								<a href="/">
									Мы
								</a>
							</li>
						</ul>
					</nav>	
                </div>
                <ul class="search-menu__options">
                    <li class="search-menu__item">
                        <a href="/" class="postponed hidden-mobile">Отложено</a>
                    </li>
                    <li class="search-menu__item hidden-mobile">
                        <a href="/" class="sign-in">Войти</a>
                    </li>
                    <li class="search-menu__item ">
                        <a href="/" class="cart"><span class="hidden-mobile">Корзина</span></a>
                    </li>
                </ul>       
            </div>
    </header>
	</div>
</template>

<style lang='scss'>
.header
{   
	margin-bottom: 30px;
	@media (max-width: 805px)
	{
			
			margin-top: -28px;
			margin-left: 5px;
			margin-bottom: 11px;

		&::after
			{
				content: '';
				position: absolute;
				height: 1px;
				background-color: #dfe0e1;
				width: 100vw;
				left: 50%;
				transform: translateX(-50%);
			}
	}
    &__contact-info
    {
    position: relative;
    display: flex;
    justify-content: space-between;
    align-items: center;
	padding-top: 16px;
    margin-block: 0px 17px;
    height: 39px;
	

		@media(max-width: 805px)
		{
			display: none;
		}
        &:first-child::after
        {
            content: '';
            position: absolute;
            height: 1px;
            background-color: #dfe0e1;
            width: 100vw;
            left: 50%;
            transform: translateX(-50%);
            bottom: -13px;
        }
    }
    
    &__delivery-list
    {
        display: flex;
        column-gap: 30px;
        font-weight: 400;
        opacity: 0.8;
    }

    &__contact-info-list
    {
        display: flex;
        column-gap: 33px;
        font-weight: 500;
        opacity: 0.8;
    }

    &__search-menu
    {
        display: flex;
        justify-content: space-between;
        align-items: center;
		height: 116px;
		@media (max-width: 805px) 
		{	
			padding-left: 5px;
			height: 98px;	
			padding-top: 27px;
		}
    }

    &__form
    {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        position: relative;
        
       

            &-input
            {

                @include fluid-form-size();
                height: var(--input-height); 
                border-radius: var(--border-radius) 0 0 var(--border-radius);
                border: var(--border-form);
                border-right: none;
                padding-left: 14px;
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
						width: 145px;
						margin-left: -10px;
						border-color: transparent;
						background-color: #f7f7f7;
					}

                &-button
                {
                    display: inline-flex;
                    align-items: center;
                    justify-content: center;
                    height: var(--button-height);
                    width:  8.6vw;
                    min-width: 50px;
                    color: var(--color-white);
                    background-color: var(--color-orange);
                    border-top-right-radius: var(--border-radius);    
                    border-bottom-right-radius: var(--border-radius);  
                    border: none;  
                    column-gap: 6px;
					@media (max-width: 805px)
					{
						background-color: #f7f7f7;
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

					&--mobile
					{
						@media (max-width: 890px){
							display: none;
						}
					}
                } 
            }
    }

    &__catalog
    {
        display: flex;
        margin-top: 20px;

        @media (max-width: 805px)
        {
            order: -1;
        }
        
        &-item:nth-child(3)
        {
            margin-left: 25px;
        }
        &-item:nth-child(4)
        {
            margin-left: 26px;
        }
        &-item:nth-child(5)
        {
            margin-left: 26px;
        }
        &-item:nth-child(6)
        {
            margin-left: 25px;
        }
        &-item:nth-child(7)
        {
            margin-left: 25px;
        }
        &-item:nth-child(2)
        {
            padding-left: 5px;
        }

        &-item--red
        {
            display: inline-flex;
            column-gap: 5px;
            justify-content: space-between;
            color: var(--color-red);

            &::before
            {
                content: '';
                background: url(./img/dekstop/svg/searh-line/label.svg) left center no-repeat;
                @include square(20px);
            }
        }
    }
}

.sign
{
    &-map
    {
        display: inline-flex;
        column-gap: 5px;
        &::before
        {
            content: '';
            background: url(./img/dekstop/svg/top-signs/map-pin.svg) left center no-repeat;
            @include square(20px);
        }
    }

    &-box
    {
        display: inline-flex;
        column-gap: 5px;
        &::before
        {
            content: '';
            background: url(./img/dekstop/svg/top-signs/ship-box.svg) left center no-repeat;
            width: 20px;
            aspect-ratio: 1;
        }
    }

    &-default
    {
        display: inline-flex;
        column-gap: 5px;
		transform: translateX(1px);

        &::before
        {
            content: '';
            background: url(./img/dekstop/svg/top-signs/address-sign.svg) left center no-repeat;
            width: 20px;
            aspect-ratio: 1;
        }
    }
}

.email
{
    display: inline-flex;
    column-gap: 7px;
	transform: translateX(2px);
    &::before
    {
        content: '';
        background: url(./img/dekstop/svg/top-signs/letter.svg) left center no-repeat;
        @include square(20px);
    }
}

.number
{
    display: inline-flex;
    column-gap: 5px;
    &::before
    {
        content: '';
        background: url(./img/dekstop/svg/top-signs/phone-sign.svg) left center no-repeat;
        @include square(20px);
    }

    &__header
    {
        &::after
        {
            content: '';
            background: url(./img/dekstop/svg/top-signs/info-sign.svg) right center no-repeat;
            @include square(20px);
        }
    }
}

.search-menu{
    display: flex;
    flex-direction: column;
    @media (max-width: 805px)
        {
            flex-direction: row;
            align-items: center;
        }

    &__logo-form
    {
        @media (max-width: 805px)
        {
            order: 2;
			margin-left: 15px;
            
        }
        &img
        {
            height: 40px;
            width: 50px;
        }

        display: flex;
        justify-content: space-between;
        column-gap: 30px;
        align-items: center;
    }

    &__options
    {
        display: flex;
        column-gap: 30px;
		margin-top: -40px;
    }
}

.postponed
{
    display: inline-flex;
    column-gap: 5px;
        &::before
            {
            content: '';
            background: url(./img/dekstop/svg/searh-line/bookmark.svg) left center no-repeat;
            @include square(20px);
            }    
}

.sign-in
{
    display: inline-flex;
    column-gap: 5px;
        &::before
            {
            content: '';
            background: url(./img/dekstop/svg/searh-line/smile.svg) left center no-repeat;
            @include square(20px);
            }    
}

.cart
{
    display: inline-flex;
    column-gap: 5px;
    position: relative;
        &::before
        {
            content: '';
            background: url(./img/dekstop/svg/searh-line/cart.svg) left center no-repeat;
            @include square(20px);
        } 
        &::after 
        {
            content: '10';
            color: var(--color-white);
            font-size: 9px;
            text-align: center;
            padding-top: 2px;
            position: absolute;
            background: var(--color-orange) no-repeat;
            left: 12px;
            border-radius: 50%;
            transform: translateY(-50%);
            @include square(15px);
        } 
			@media (max-width: 805px)
			{
				transform: translate(-14px, 23px);
				
				&::before
				{
					content: '';
					background: url(./img/dekstop/svg/searh-line/cart.svg) left center no-repeat;
					background-size: 25px;
					@include square(25px);
				} 
				&::after 
				{
					content: '10';
					color: var(--color-white);
					font-size: 13px;
					text-align: center;
					padding-top: 1px;
					position: absolute;
					background: var(--color-orange) no-repeat;
					background-size: 25px;
					left: 12px;
					border-radius: 50%;
					transform: translateY(-50%);
					@include square(20px);
				}
			}
		
        
}

.catalog-sign
{
    @include square(20px);
	@media (max-width: 805px)
    {
        padding-bottom: 20px;
    }

}

.big-logo
{
    flex: 0 0 auto;
    @media (max-width: 805px)
    {
        width: 43px;
        height: 35px;
    }
    @media (min-width: 805px)
    {
        width: 50px;
        height: 40px;
    }
}

.white-bc
{
	background-color: #fff;	

}

html
{
	overflow-y: scroll;
	@media (max-width: 805)
	{
		overflow-y: scroll;
	}
}





</style>