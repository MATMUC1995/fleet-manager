# 🚗 Fleet Manager

Fleet Manager to aplikacja webowa typu CRUD stworzona w PHP (Symfony) do zarządzania flotą pojazdów i przypisanymi do nich pracownikami.

## 🛠 Technologie

- PHP 8.2
- Symfony 6
- Doctrine ORM
- MySQL/MariaDB
- API Platform (REST)
- Docker/XAMPP (opcjonalnie)
- PHPStan + Intelephense
- Bootstrap 5 (frontend)

## 🧑‍💻 Funkcjonalności

- Dodawanie/edycja/usuwanie pojazdów
- Dodawanie/edycja/usuwanie pracowników
- Przypisywanie pojazdów do użytkowników
- System wiadomości (Messenger)
- REST API (dla pojazdów i użytkowników)

## ✅ Wymagania

- PHP >= 8.1
- Composer
- MySQL / MariaDB
- Symfony CLI (opcjonalnie)
- XAMPP lub Docker (opcjonalnie)

## 🚀 Instalacja i uruchomienie

```bash
git clone https://github.com/TWOJ-LOGIN/fleet-manager.git
cd fleet-manager
composer install
cp .env .env.local


Skonfiguruj bazę danych w .env.local (np. dla XAMPP):
DATABASE_URL="mysql://root:@127.0.0.1:3306/fleet_manager?serverVersion=10.4"

php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate

php bin/console doctrine:fixtures:load

symfony server:start
```
Aplikacja będzie dostępna pod https://127.0.0.1:8000.

## 🧪TESTS
```bash
php bin/phpunit
```
📂 Struktura projektu
src/Entity – encje Doctrine

src/Repository – zapytania do bazy danych

src/Controller – kontrolery API

src/DataPersister – niestandardowe zapisujące dane

config/ – konfiguracja aplikacji

public/ – katalog publiczny (dla serwera)




## 📫 Kontakt

Autor: Mateusz

Email: matmuc1995@gmail.com

GitHub: https://github.com/MATMUC1995


