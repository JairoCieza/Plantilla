# Plantilla Laravel Inertia + Vue3

Este proyecto es una guía para crear una aplicación en Laravel 10 con las siguientes características:

1. **Instalación de Laravel Breeze** con Inertia.js y Vue 3.
2. **Integración de Bootstrap 5** como framework CSS.
3. **Gestión de roles y permisos** mediante [spatie/laravel-permission](https://github.com/spatie/laravel-permission).
4. CRUD de **Usuarios**, **Roles** y **Módulos**.
5. **Sidebar** estilo AdminLTE cargado dinámicamente desde base de datos según el rol del usuario autenticado.
6. **Gráfico de barras** en el dashboard usando Chart.js que muestre la cantidad de usuarios por rol.
7. Interfaz completamente en español.
8. Seeders con roles, usuarios de prueba, módulos iniciales y relaciones.

## Pasos para instalar

1. Clonar este repositorio.
2. Crear el proyecto con Composer:
   ```bash
   composer create-project laravel/laravel="^10.0" .
   ```
3. Instalar Breeze con Inertia y Vue:
   ```bash
   php artisan breeze:install vue
   npm install && npm run build
   ```
4. Instalar spatie/laravel-permission:
   ```bash
   composer require spatie/laravel-permission
   php artisan vendor:publish --provider="Spatie\Permission\PermissionServiceProvider"
   php artisan migrate
   ```
5. Configurar Bootstrap 5 y Chart.js en `resources/js/app.js`.
6. Implementar los CRUD mencionados y el sidebar dinámico.
7. Crear los seeders para roles, usuarios y módulos.
8. Ejecutar las migraciones y seeders:
   ```bash
   php artisan migrate --seed
   ```

## Uso

Una vez instalado, inicie el servidor con:
```bash
php artisan serve
```

## Notas

Este repositorio solo incluye instrucciones básicas. Los archivos de Laravel no se encuentran en el entorno actual.
