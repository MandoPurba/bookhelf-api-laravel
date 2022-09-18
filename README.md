<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<h1 align="center">
Bookhelf API Laravel
</h1>

## Instalation
> Run `composer install` di terminal

## Create Database
> Buat database `bookhelf_api_laravel` atau edit file `.env`
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306 //Port Database anda
DB_DATABASE=bookhelf_api_laravel //Nama database anda
DB_USERNAME=root //Username database anda
DB_PASSWORD= //password database anda
```
## Migrasi
> Jalankan migrasi dengan perintah `php artisan migrate` di terminal

## Jalankan aplikasi
> jalankan aplikasi di lokal server dengan perintah `php artisan serve` di terminal

## Pengujian di Postman
> ### 1. Ambil data
> Method: GET <br>
> URL: http:localhost:8000/api/book

> ### 2. Tambah data
> Method: POST <br>
> URL: http:localhost:8000/api/book
> ```{
>       "title": "Laravel 2",
>       "year": 2020,
>       "author": "Mando Purba",
>       "summary": "rhoncus est pellentesque elit ullamcorper dignissim cras tincidunt lobortis feugiat vivamus at augue eget arcu",
>       "publisher": "SayaSendiri",
>       "page_count": 120,
>       "read_page": 1,
>       "reading": 0
>   }```
    
> ### 3. Update data
> Method: PUT<br>
> URL: http:localhost:8000/api/books/<i>{id_buku}</i>
> ```{
>       "title": "Laravel 2 update",
>       "year": 2020,
>       "author": "Mando Purba",
>       "summary": "rhoncus est pellentesque elit ullamcorper dignissim cras tincidunt lobortis feugiat vivamus at augue eget arcu",
>       "publisher": "SayaSendiri",
>       "page_count": 120,
>       "read_page": 1,
>       "reading": 0
>   }```

> ### 4. Delete data
> Method: DELETE
> URL: http:localhost:8000/api/books/<i>{id_buku}</i>
