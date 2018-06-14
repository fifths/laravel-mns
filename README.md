# laravel-mns

Version 1.3.5

## Install

```
composer require fifths/laravel-mns
```


## Lumen
```
$app->register(LaravelMNS\LaravelMNSServiceProvider::class);
```

## config/queue.php
```
        'mns' => [
            'driver' => 'mns',
            'key' => env('QUEUE_MNS_ACCESS_KEY_ID'),
            'secret' => env('QUEUE_MNS_ACCESS_KEY_SECRET'),
            'endpoint' => env('QUEUE_MNS_ENDPOINT'),
            'queue' => 'default',
            'wait_seconds' => 30,
        ],
```

## .env
```
# QUEUE MNS
QUEUE_DRIVER=mns
QUEUE_MNS_ACCESS_KEY_ID=
QUEUE_MNS_ACCESS_KEY_SECRET=
QUEUE_MNS_ENDPOINT=
```