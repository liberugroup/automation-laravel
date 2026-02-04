# Liberu Automation

[Managed web hosting for our application packages](https://liberu.co.uk)

[![PHP](https://img.shields.io/badge/PHP-8.4-informational?style=flat&logo=php&color=4f5b93)](https://www.php.net/)
[![Laravel](https://img.shields.io/badge/Laravel-12-informational?style=flat&logo=laravel&color=ef3b2d)](https://laravel.com/)
[![Filament](https://img.shields.io/badge/Filament-4.0-informational?style=flat&color=fdae4b&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSI0OCIgaGVpZ2h0PSI0OCIgeG1sbnM6dj0iaHR0cHM6Ly92ZWN0YS5pby9uYW5vIj48cGF0aCBkPSJNMCAwaDQ4djQ4SDBWMHoiIGZpbGw9IiNmNGIyNWUiLz48cGF0aCBkPSJNMjggN2wtMSA2LTMuNDM3LjgxM0wyMCAxNWwtMSAzaDZ2NWgtN2wtMyAxOEg4Yy41MTUtNS44NTMgMS40NTQtMTEuMzMgMy0xN0g4di01bDUtMSAuMjUtMy4yNUMxNCAxMSAxNCAxMSAxNS40MzggOC41NjMgMTkuNDI5IDYuMTI4IDIzLjQ0MiA2LjY4NyAyOCA3eiIgZmlsbD0iIzI4MjQxZSIvPjxwYXRoIGQ9Ik0zMCAxOGg0YzIuMjMzIDUuMzM0IDIuMjMzIDUuMzM0IDEuMTI1IDguNUwzNCAyOWMtLjE2OCAzLjIwOS0uMTY4IDMuMjA5IDAgNmwtMiAxIDEgM2gtNXYyaC0yYy44NzUtNy42MjUuODc1LTcuNjI1IDItMTFoMnYtMmgtMnYtMmwyLTF2LTQtM3oiIGZpbGw9IiMyYTIwMTIiLz48cGF0aCBkPSJNMzUuNTYzIDYuODEzQzM4IDcgMzggNyAzOSA4Yy4xODggMi40MzguMTg4IDIuNDM4IDAgNWwtMiAyYy0yLjYyNS0uMzc1LTIuNjI1LS4zNzUtNS0xLS42MjUtMi4zNzUtLjYyNS0yLjM3NS0xLTUgMi0yIDItMiA0LjU2My0yLjE4N3oiIGZpbGw9IiM0MDM5MzEiLz48cGF0aCBkPSJNMzAgMThoNGMyLjA1NSA1LjMxOSAyLjA1NSA1LjMxOSAxLjgxMyA4LjMxM0wzNSAyOGwtMyAxdi0ybC00IDF2LTJsMi0xdi00LTN6IiBmaWxsPSIjMzEyODFlIi8+PHBhdGggZD0iTTI5IDI3aDN2MmgydjJoLTJ2MmwtNC0xdi0yaDJsLTEtM3oiIGZpbGw9IiMxNTEzMTAiLz48cGF0aCBkPSJNMzAgMThoNHYzaC0ydjJsLTMgMSAxLTZ6IiBmaWxsPSIjNjA0YjMyIi8+PC9zdmc+)
[![Livewire](https://img.shields.io/badge/Livewire-latest-informational?style=flat&color=fb70a9)](https://laravel-livewire.com/)
[![Socialite](https://img.shields.io/badge/Socialite-latest-brightgreen.svg)](https://laravel.com/docs/socialite)

[![Install workflow](https://github.com/liberu-automation/automation-laravel/actions/workflows/install.yml/badge.svg)](https://github.com/liberu-automation/automation-laravel/actions/workflows/install.yml)
[![Tests workflow](https://github.com/liberu-automation/automation-laravel/actions/workflows/tests.yml/badge.svg)](https://github.com/liberu-automation/automation-laravel/actions/workflows/tests.yml)
[![Docker workflow](https://github.com/liberu-automation/automation-laravel/actions/workflows/main.yml/badge.svg)](https://github.com/liberu-automation/automation-laravel/actions/workflows/main.yml)
[![Codecov](https://codecov.io/gh/liberu-automation/automation-laravel/branch/main/graph/badge.svg)](https://codecov.io/gh/liberu-automation/automation-laravel)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

A lightweight Laravel-based control panel for automated hosting and billing workflows. Designed for maintainability and integration with Filament and Jetstream.

**Key features**

- Hosting control panel primitives (user, team, account, site settings)
- Billing automation hooks and seeders
- Filament admin resources and Livewire components
- Pluggable modules architecture

## Quick start

1. Requirements: PHP 8.3+, Composer, Node.js (optional for assets).
2. Clone the repository and install dependencies.

PowerShell / Bash

```powershell
# install PHP deps, generate key, migrate and seed
composer install; 
cp .env.example .env; 
php artisan key:generate; 
php artisan migrate --seed
```

Docker (build & run)

```bash
# build image and run (local, single-container)
docker build -t automation-laravel .; 
docker run -p 8000:8000 automation-laravel
```

Using Laravel Sail

```bash
# start Sail (Docker)
./vendor/bin/sail up -d
```

## Related projects

| Project | Repository |
|---|---|
| Accounting | [liberu-accounting/accounting-laravel](https://github.com/liberu-accounting/accounting-laravel) |
| Automation (this) | [liberu-automation/automation-laravel](https://github.com/liberu-automation/automation-laravel) |
| Billing | [liberu-billing/billing-laravel](https://github.com/liberu-billing/billing-laravel) |
| Boilerplate | [liberusoftware/boilerplate](https://github.com/liberusoftware/boilerplate) |
| Browser game | [liberu-browser-game/browser-game-laravel](https://github.com/liberu-browser-game/browser-game-laravel) |
| CMS | [liberu-cms/cms-laravel](https://github.com/liberu-cms/cms-laravel) |
| Control Panel | [liberu-control-panel/control-panel-laravel](https://github.com/liberu-control-panel/control-panel-laravel) |
| CRM | [liberu-crm/crm-laravel](https://github.com/liberu-crm/crm-laravel) |
| E-commerce | [liberu-ecommerce/ecommerce-laravel](https://github.com/liberu-ecommerce/ecommerce-laravel) |
| Genealogy | [liberu-genealogy/genealogy-laravel](https://github.com/liberu-genealogy/genealogy-laravel) |
| Maintenance | [liberu-maintenance/maintenance-laravel](https://github.com/liberu-maintenance/maintenance-laravel) |
| Real estate | [liberu-real-estate/real-estate-laravel](https://github.com/liberu-real-estate/real-estate-laravel) |
| Social network | [liberu-social-network/social-network-laravel](https://github.com/liberu-social-network/social-network-laravel) |

## Contributing

- Please open issues for bugs or feature requests.
- Contributions are welcome via pull requests. Follow PSR-12 coding style and include tests where applicable.

## License

This project is released under the MIT License. See the `LICENSE` file for details.

<div align="center">Made with ♥ by Liberu</div>
