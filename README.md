## Configuration Setup

- composer create-project laravel/laravel chat-application [create new project with name chat-application]
- npm install -g @vue/cli [globally installed npm package and provides the vue command in terminal]
- composer require laravel/ui  ===> [laravel ui -> easy to make vue aurthentication system]
- php artisan ui vue --auth
- npm install vue@next vue-loader@next [installl vue v3 only if different in composer.json file]
- run command => npm run watch -> [if "mix" error then do these steps:  
										1) delete package-lock.json  manually
										2) remove nodemodules by cmd => rm -rf node_modules
										3) npm install

## Setup pusher

- copy .env.example file as .env
- setup environment variables that are mentioned below:
    PUSHER_APP_ID=my_pusher_app_id
    PUSHER_APP_KEY=my_pusher_app_key
    PUSHER_APP_SECRET=my_pusher_app_secret
    PUSHER_HOST=127.0.0.1
    PUSHER_PORT=6001
    PUSHER_SCHEME=http
    PUSHER_APP_CLUSTER=mt1
-uncomment broadcastServiceProvider from providers from app.php in config folder
        App\Providers\BroadcastServiceProvider::class,

## To run project

- php artisan serve 
- php artisan websockets:serve
- npm run watch 


## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions) as well as [websockets] (https://beyondco.de/docs/laravel-websockets)

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
# chat-application
