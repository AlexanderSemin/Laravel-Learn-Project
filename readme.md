<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

1)install laravel in current directory
	
	ставим ларавел в текущей директории вот такой вот командой
	
	composer create-project --prefer-dist laravel/laravel . "5.5.*"

2)создание миграций
	
	php artisan make:migration create_categories_table --create=categories
	php artisan make:migration create_articles_table --create=articles
	php artisan make:migration ...... и  т.д.
	
	прописываем в файлах миграций все необходимые поля которые нам будут нужны
	
	
3)создаем базу
 
	CREATE SCHEMA `laravel-blog` DEFAULT CHARACTER SET utf8 ;

4)указываем подключение к бд   в файле .ENV

	DB_CONNECTION=mysql
	DB_HOST=127.0.0.1
	DB_PORT=3306
	DB_DATABASE=laravel-blog
	DB_USERNAME=root
	DB_PASSWORD=1111

5)выполняем ВСЕ миграции командой 

    php artisan migrate





### License
The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
