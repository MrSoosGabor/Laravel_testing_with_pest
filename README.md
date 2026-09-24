## Laravel Testing With Pest

**Created By :** malagi
**Email :** malagi@gmail.com

## Installation

To get started, clone this repository.

```
git clone https://github.com/MrSoosGabor/Laravel_testing_with_pest.git
```

Next, copy your `.env.example` file as `.env` and configure your Database connection.

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=YOUR-DATABASE-NAME
DB_USERNAME=YOUR-DATABASE-USERNAME
DB_PASSWORD=YOUR-DATABASE-PASSWORD
```

## Run Packages and helpers

You have to all used packages and load helpers as below.

```
composer install
npm install
npm run build
```

## Generate new application key

You have to generate new application key as below.

```
php artisan key:generate
```

## Run Migrations and Seeders

You have to run all the migration files included with the project and also run seeders as below.

```
php artisan migrate
php artisan db:seed
```

## Project Execution

```
php artisan serve
```


## A `pa` rövidítés beállítása Windows alatt

Ha nem szeretnéd minden alkalommal kiírni a `php artisan` szöveget, hozz létre egy
`pa` rövidítést a terminálban. Ezután például a `php artisan migrate` helyett a
`pa migrate` parancsot használhatod.

### PowerShell esetén (tartós beállítás)

1. Nyisd meg a PowerShell profilfájlját:

```powershell
notepad $PROFILE
```

2. Add hozzá ezt a sort:

```powershell
function pa { php artisan $args }
```

3. Mentsd el a fájlt, majd indítsd újra a terminált. Ha a profilfájl még nem
létezik, előbb hozd létre:

```powershell
New-Item -ItemType File -Path $PROFILE -Force
notepad $PROFILE
```

Ellenőrzés:

```powershell
pa --version
```

### CMD esetén (az aktuális terminálhoz)

A CMD-ben futtasd:

```cmd
doskey pa=php artisan $*
```

Ez a rövidítés csak az aktuális CMD-ablak bezárásáig él. Ezután használhatod
például így:

```cmd
pa migrate
pa db:seed
pa serve
```

VS Code-ban Markdown előnézet megnyitása:

Ctrl + Shift + V – előnézet az aktuális fülön
Ctrl + K, majd V – előnézet új oldalsó panelen
A Markdown fájl szerkesztőnézetébe az Esc billentyűvel térhetsz vissza.
