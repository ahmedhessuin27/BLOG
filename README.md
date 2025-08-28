# Laravel Blog System

<p align="center">
<img src="https://img.shields.io/badge/Laravel-10.x-red.svg" alt="Laravel Version">
<img src="https://img.shields.io/badge/PHP-8.1+-blue.svg" alt="PHP Version">
<img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
<img src="https://img.shields.io/badge/Status-Development-yellow.svg" alt="Status">
</p>

A modern, multilingual blog platform built with Laravel 10, featuring content management, multi-language support, and a clean, responsive design.

## 🚀 Features

- **Multilingual Support**: Built-in localization with Arabic and English support
- **Content Management**: Create, edit, and manage blog posts and categories
- **User Authentication**: Secure user registration and login system with Laravel Breeze
- **Responsive Design**: Modern UI with Tailwind CSS
- **Translation Management**: Manage content in multiple languages
- **Category System**: Organize posts with categories
- **User Profiles**: User profile management system
- **Soft Deletes**: Safe deletion with recovery options
- **Modern Frontend**: Vite + Alpine.js for enhanced user experience

## 🛠️ Technology Stack

### Backend
- **Laravel 10**: PHP web framework
- **PHP 8.1+**: Modern PHP features
- **MySQL**: Database management
- **Laravel Sanctum**: API authentication
- **Laravel Breeze**: Authentication scaffolding

### Frontend
- **Tailwind CSS**: Utility-first CSS framework
- **Alpine.js**: Lightweight JavaScript framework
- **Vite**: Fast build tool
- **Blade Templates**: Laravel's templating engine

### Key Packages
- **Astrotomic/Laravel-Translatable**: Multi-language content support
- **Mcamara/Laravel-Localization**: URL localization
- **Laravel Sail**: Docker development environment

## 📋 Prerequisites

- PHP 8.1 or higher
- Composer
- Node.js & NPM
- MySQL/MariaDB
- Git

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ahmedhessuin27/BLOG.git
   cd BLOG
   ```

2. **Install PHP dependencies**
   ```bash
   composer install
   ```

3. **Install Node.js dependencies**
   ```bash
   npm install
   ```

4. **Environment setup**
   ```bash
   copy .env.example .env
   php artisan key:generate
   ```

5. **Configure database**
   Update your `.env` file with database credentials:
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=blog
   DB_USERNAME=your_username
   DB_PASSWORD=your_password
   ```

6. **Run migrations**
   ```bash
   php artisan migrate
   ```

7. **Seed the database (optional)**
   ```bash
   php artisan db:seed
   ```

8. **Build assets**
   ```bash
   npm run build
   ```

9. **Start the development server**
   ```bash
   php artisan serve
   ```

Visit `http://localhost:8000` to view the application.

## 🗄️ Database Structure

### Core Tables
- **users**: User authentication and profiles
- **categories**: Blog post categories
- **category_translations**: Category translations
- **posts**: Blog posts
- **post_translations**: Post translations
- **settings**: Application settings

### Translation Support
The application uses the Translatable package to support multiple languages:
- Arabic (ar)
- English (en)

## 🎯 Usage

### Content Management
1. **Creating Posts**: Navigate to the dashboard to create new blog posts
2. **Managing Categories**: Organize content with category management
3. **Translations**: Add content in multiple languages
4. **User Management**: Manage user profiles and authentication

### Development
- **Assets**: Run `npm run dev` for development with hot reloading
- **Testing**: Run `php artisan test` to execute the test suite
- **Code Style**: Use `./vendor/bin/pint` for code formatting

## 🧪 Testing

Run the test suite:
```bash
php artisan test
```

Run specific test files:
```bash
php artisan test --filter ProfileTest
```

## 📁 Project Structure

```
├── app/
│   ├── Http/Controllers/     # Application controllers
│   ├── Models/              # Eloquent models
│   └── Providers/           # Service providers
├── database/
│   ├── migrations/          # Database migrations
│   └── seeders/            # Database seeders
├── resources/
│   ├── views/              # Blade templates
│   ├── css/                # Stylesheets
│   └── js/                 # JavaScript files
├── routes/                 # Application routes
└── tests/                  # Test files
```

## 🌐 Localization

The application supports multiple languages:
- **Arabic**: Default RTL support
- **English**: Full translation support

### Adding New Languages
1. Add language files in `resources/lang/`
2. Update the translatable configuration
3. Create translation records in the database

## 🚀 Deployment

### Production Setup
1. **Environment**: Set `APP_ENV=production` in `.env`
2. **Optimize**: Run optimization commands:
   ```bash
   php artisan config:cache
   php artisan route:cache
   php artisan view:cache
   ```
3. **Assets**: Build production assets:
   ```bash
   npm run build
   ```

### Server Requirements
- PHP 8.1+
- MySQL 5.7+
- Composer
- Web server (Apache/Nginx)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## 👨‍💻 Author

**Ahmed Hussain** - [GitHub Profile](https://github.com/ahmedhessuin27)

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Contact the development team

---

**Built with ❤️ using Laravel & Tailwind CSS**
