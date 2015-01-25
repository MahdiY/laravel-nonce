#This is a Laravel package for using Nonces for HTTP Requests.

Instalation:

Using Composer, just add 
```
"vjroby/laravel-nonce": "dev-master"
```
to your `compsoer.json` file and run a compposer update

add to app providers:

```
'Vjroby\LaravelNonce\LaravelNonceServiceProvider'
```

and to aliases:

```
'Nonce'			=> 'Vjroby\Facade\NonceFacade',
```

so it can be used as static class in the project.

For creating the table:

`php artisan vjroby-laravel-nonce:migrations`

It will create `2014_12_18_133440_create_nonce_table migration.php` file,

and then:

`php artisan migrate`


