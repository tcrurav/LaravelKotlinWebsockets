# Using Websockets in Laravel (Backend) and Android Kotlin (frontend)

It's just that... an example using Websockets in Laravel (Backend) and Android Kotlin (frontend)

And now shows quite nothing but the connection. This is just the beginning...

## Prerequisites

You need a working environment with:
* [Git](https://git-scm.com) - You can install it from https://git-scm.com/downloads.
* [MySQL](https://www.mysql.com) - You can install it from https://www.mysql.com/downloads/.
* [Laravel](https://laravel.com/) - Laravel is a web application framework with expressive, elegant syntax.
* [Android Studio](https://developer.android.com/studio?hl=es) - Android Studio provides the fastest tools for building apps on every type of Android device.

## General Installation instructions

The best option to start with this project is cloning it in your PC:

```
git clone https://github.com/tcrurav/LaravelKotlinWebsockets.git
```

This project contains 2 different parts:
* Frontend (Open and run it with Android Studio)
* Backend (laravel)

In the backend use the following .env file:

```
APP_NAME=Laravel
APP_ENV=local
APP_KEY=base64:3zAznbgqAah9JQsRD/sjP99Mr9ttFDxA/NI1g2FNpAk=
APP_DEBUG=true
APP_URL=http://localhost

LOG_CHANNEL=stack
LOG_LEVEL=debug

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravelwebsockets
DB_USERNAME=pepe
DB_PASSWORD=sasa

BROADCAST_DRIVER=pusher
CACHE_DRIVER=file
QUEUE_CONNECTION=sync
SESSION_DRIVER=file
SESSION_LIFETIME=120

MEMCACHED_HOST=127.0.0.1

REDIS_HOST=127.0.0.1
REDIS_PASSWORD=null
REDIS_PORT=6379

MAIL_MAILER=smtp
MAIL_HOST=mailhog
MAIL_PORT=1025
MAIL_USERNAME=null
MAIL_PASSWORD=null
MAIL_ENCRYPTION=null
MAIL_FROM_ADDRESS=null
MAIL_FROM_NAME="${APP_NAME}"

AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_DEFAULT_REGION=us-east-1
AWS_BUCKET=

PUSHER_APP_ID=123456
PUSHER_APP_KEY=12345asdfasdf
PUSHER_APP_SECRET=12345asdfasdf
PUSHER_APP_CLUSTER=mt1

MIX_PUSHER_APP_KEY="${PUSHER_APP_KEY}"
MIX_PUSHER_APP_CLUSTER="${PUSHER_APP_CLUSTER}"

YOUR_LOCAL_IP=192.168.0.23
```

Don't forget to put your local IP Address in the following places:
* frontend: in the file MainActivity.kt
* backend: in the file broadcasting.php

Interesting detail to find out the URL to connect to:

![Create Project](/docs/screenshots/ParaJavierMedinaYNéstorCabanillas-1.png)

![Create Project](/docs/screenshots/ParaJavierMedinaYNéstorCabanillas-2.png)

## Built With

* [Visual Studio Code](https://code.visualstudio.com/) - The Editor used in this project
* [MySQL](https://www.mysql.com) - You can install it from https://www.mysql.com/downloads/.
* [Laravel](https://laravel.com/) - Laravel is a web application framework with expressive, elegant syntax.
* [Android Studio](https://developer.android.com/studio?hl=es) - Android Studio provides the fastest tools for building apps on every type of Android device.
* [MySQL Workbench](https://www.mysql.com/products/workbench/) - MySQL Workbench is a unified visual tool for database architects, developers, and DBAs.
* [dotenv](https://www.npmjs.com/package/dotenv) - Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env. Storing configuration in the environment separate from code is based on The Twelve-Factor App methodology.

## Acknowledgments

* https://beyondco.de/docs/laravel-websockets/getting-started/introduction. Laravel BeyondCode websockets library used in this project.
* https://medium.com/swlh/android-tutorial-part-1-using-java-websocket-with-kotlin-646a5f1f09de. Tutorial followed in this project for the frontend.
* https://alejandroroa.medium.com/laravel-websockets-a5573e38301d. A very good tutorial to start with websockets in laravel.