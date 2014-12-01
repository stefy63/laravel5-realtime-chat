# Laravel Realtime Chat

A realtime chat sample written in Laravel 4.2 + Redis + Node.js + Socket.io.

Um exemplo de chat realtime escrito em Laravel 4.2 + Redis Node.js + Socket.io (instruções somente em inglês).

##Requirements
	Laravel 4.2
	MySQL
	Redis
	Node.js
	NPM

##How to install
### Step 1: Clone this repo

```bash
$ git clone https://github.com/guilhermeslk/laravel-realtime-chat.git
```
### Step 2: Install composer packages

```bash
$ cd laravel-realtime-chat
$ composer install
```
### Step 3: Configure Database
Edit your ***app/config/local/database.php*** to match your local database settings.

### Step 4: Migrate & Populate Database
Run these commands to create and populate your database:

```bash
$ php artisan migrate
$ php artisan db:seed
```

### Step 5: Install NPM dependencies
CD into the nodejs folder and run npm install in order to have the all dependencies installed.

```bash
$ cd nodejs
$ npm install
```

### Step 6: Run PHP's built-in development server

```bash
$ cd ..
$ php artisan serve
```
### Step 7: Start Redis Server

```bash
$ redis-server
```

### Step 8: Start the "Realtime" server (nodejs/server.js)

```bash
$ ./realtime.sh
```

That's it! Now you should be ready to go!
