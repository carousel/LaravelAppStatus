[miroslav.trninic@gmail.com](mailto:miroslav.trninic@gmail.com)

If you are on the server, this simple artisan command will tell you if the application is UP or DOWN, without visiting browser.


INSTRUCTIONS:

1. Copy file into app/Console/Commands directory
2. Add this line in app/Console/Kernel.php file:
```
    protected $commands = [
            //other commands 
            'App\Console\Commands\AppStatusCommand',
    ];
```
3. Use builtin Laravel command **php artisan down/up** and check status of your app by  running **php artisan status**

