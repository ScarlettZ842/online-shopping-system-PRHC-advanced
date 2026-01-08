![GitHub](https://img.shields.io/github/license/puneethreddyhc/online-shopping-system-advanced)
![](https://visitor-badge.glitch.me/badge?page_id=puneethreddyhc.onlineadv)

<a href="https://www.buymeacoffee.com/puneethreddyhc" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" width="195" height="55"></a>

> ## Updated project with extra Features like WISHLIST, List Orders, add Reviews, updated routing, resolved search bug is available for Premium

[![Youtube Video](https://img.youtube.com/vi/gLwfj67GI8A/0.jpg)](https://youtu.be/gLwfj67GI8A)

<h3>Things I code with</h3>
<p>
  <img alt="npm" src="https://img.shields.io/badge/-NPM-CB3837?style=flat-square&logo=npm&logoColor=white" />
  <img alt="html5" src="https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/static/v1?label=Vue.js&amp;message=v2.6&amp;color=4FC08D&amp;style=flat-square&amp;logo=vue.js&amp;logoColor=ffffff" alt="vue.js">
  <img alt="Django" src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" />
  <img alt="Flutter" src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" />
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E" />
  <img alt="Mysql" src="https://img.shields.io/badge/MySQL-00000F?style=flat-square&logo=mysql&logoColor=white" />
  <img alt="postgresql" src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" />
  <img alt="Amazon_AWS" src="https://img.shields.io/badge/Amazon_AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white" />
  <img alt="Css" src="https://img.shields.io/badge/CSS-239120?&style=flat-square&logo=css3&logoColor=white" />
  <img alt="Sass" src="https://img.shields.io/badge/-Sass-CC6699?style=flat-square&logo=sass&logoColor=white" />
  <img alt="Styled Components" src="https://img.shields.io/badge/-Styled_Components-db7092?style=flat-square&logo=styled-components&logoColor=white" />
  <img alt="git" src="https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img alt="Heroku" src="https://img.shields.io/badge/-Heroku-430098?style=flat-square&logo=heroku&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-46a2f1?style=flat-square&logo=docker&logoColor=white" />
  <img alt="angular" src="https://img.shields.io/badge/-Angular-DD0031?style=flat-square&logo=angular&logoColor=white" />
  <img alt="MongoDB" src="https://img.shields.io/badge/-MongoDB-13aa52?style=flat-square&logo=mongodb&logoColor=white" />
  <img alt="Nodejs" src="https://img.shields.io/badge/-Nodejs-43853d?style=flat-square&logo=Node.js&logoColor=white" />
  <img alt="Google Cloud Platform" src="https://img.shields.io/badge/-Google_Cloud_Platform-1a73e8?style=flat-square&logo=google-cloud&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/-TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white" />
  
</p>
<h1>Projects We develop</h1>

<ul>
	<li><b>Vue JS</b></li>
	<li><b>Nuxt JS</b></li>
	<li><b>Python</b></li>
	<li><b>Django</b></li>
	<li><b>PHP and MYSQL</b></li>
	<li><b>Angular JS</b></li>
	<li><b>React JS</b></li>
	<li><b>AI/ML</b></li>
</ul>
<h2> Projects with installation support and code explaination for Premium contact gmail: puneethreddy951@gmail.com or visit :<a href="http://www.projectswall.com/">Projects Wall</a></h2>

# Installation

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Docker Desktop** (for macOS/Windows) or **Docker Engine** (for Linux)
- **Docker Compose** (included with Docker Desktop)

### Installing Docker

#### macOS / Windows:

1. Download Docker Desktop from [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)
2. Install and start Docker Desktop
3. Verify installation: `docker --version` and `docker compose version`

#### Linux:

```bash
# Install Docker
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh

# Install Docker Compose
sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

---

## Quick Start with Docker (Recommended)

### 1. Clone the Repository

```bash
git clone https://github.com/PuneethReddyHC/online-shopping-system-with-advanced-admin-page.git
cd online-shopping-system-PRHC-advanced
```

### 2. Start the Application

```bash
docker compose up -d
```

That's it! The entire application (web server + database) will be up and running.

### 3. Access the Application

- **Main Website**: http://localhost:8080
- **Admin Panel**: http://localhost:8080/admin/admin/

---

## Docker Commands Reference

### Essential Commands

```bash
# Start the application
docker compose up -d

# Stop the application
docker compose down

# Restart the application
docker compose restart

# View logs
docker compose logs -f

# View running containers
docker compose ps

# Stop and remove all data (including database)
docker compose down -v

# Rebuild containers (after Dockerfile changes)
docker compose up -d --build
```

### Troubleshooting Commands

```bash
# Check database logs
docker logs onlineshop_db_advanced

# Check web server logs
docker logs onlineshop_web_advanced

# Access database directly
docker exec -it onlineshop_db_advanced mysql -u root onlineshop

# Access web container shell
docker exec -it onlineshop_web_advanced bash
```

---

## Database Information

### MySQL Container Details

- **Host**: `db` (within Docker network) or `localhost` (from host machine)
- **Port**: `3306`
- **Database Name**: `onlineshop`
- **Username**: `root`
- **Password**: _(empty)_
- **Image**: MySQL 8.0

### Database Schema

The database is automatically initialized from `database/onlineshop.sql` on first run. It includes:

- **Admin accounts** (`admin_info`)
- **User accounts** (`user_info`, `user_info_backup`)
- **Products catalog** (`products`, `categories`, `brands`)
- **Shopping cart** (`cart`, `wishlist`)
- **Orders** (`orders`, `orders_info`, `order_products`)
- **Reviews** (`reviews`)
- **Email subscriptions** (`email_info`)
- **Activity logs** (`logs`)

### Access MySQL from Host

```bash
mysql -h 127.0.0.1 -P 3306 -u root onlineshop
```

Or use any MySQL client (MySQL Workbench, phpMyAdmin, etc.) with:

- Host: `127.0.0.1`
- Port: `3306`
- User: `root`
- Password: _(leave empty)_
- Database: `onlineshop`

---

## Application Features

### Customer Features

- 🛍️ **Browse Products** - View products by category and brand
- 🔍 **Search & Filter** - Advanced search with filters
- 🛒 **Shopping Cart** - Add/remove items, update quantities
- ❤️ **Wishlist** - Save products for later
- 👤 **User Account** - Registration and login
- 📦 **Order Management** - View order history
- ⭐ **Product Reviews** - Rate and review products
- 💳 **Checkout Process** - Complete purchase flow

### Admin Features

- 📊 **Dashboard** - Overview of sales and activities
- ➕ **Product Management** - Add, edit, delete products
- 👥 **User Management** - Manage customer accounts
- 📋 **Order Management** - View and manage orders
- 📈 **Sales Reports** - Daily sales tracking
- ⚙️ **System Settings** - Configure application settings

---

## Login Credentials

### Admin Account

- **Email**: `admin@gmail.com`
- **Username**: `admin`
- **Password**: `123456789`

### Test User Account

- **Email**: `otheruser@gmail.com`
- **Username**: `otheruser`
- **Password**: `support`

---

## Docker Architecture

The application consists of two containers:

### 1. Web Container (`onlineshop_web_advanced`)

- **Base Image**: PHP 8.0 with Apache
- **Port**: 8080 → 80
- **Features**:
  - PHP with mysqli extension
  - Apache mod_rewrite enabled
  - Live code mounting for development

### 2. Database Container (`onlineshop_db_advanced`)

- **Base Image**: MySQL 8.0
- **Port**: 3306 → 3306
- **Features**:
  - Persistent data storage
  - Automatic schema initialization
  - Health checks

### Docker Volumes

- `db_data`: Persists database data between container restarts

### Docker Network

- `shop_network`: Bridge network connecting web and database containers

---

## Environment Variables

The application uses the following environment variables (set in `docker-compose.yml`):

```yaml
DB_HOST=db          # Database hostname
DB_USER=root        # Database user
DB_NAME=onlineshop  # Database name
```

Password is left empty as per original configuration.

---

## File Structure

```
.
├── docker-compose.yml          # Docker Compose configuration
├── Dockerfile                  # Web server image definition
├── .dockerignore              # Files excluded from Docker build
├── DOCKER.md                  # Detailed Docker documentation
├── database/
│   └── onlineshop.sql         # Database schema and seed data
├── admin/                     # Admin panel files
│   ├── admin/                 # Admin dashboard
│   │   ├── index.php         # Admin home
│   │   ├── add_products.php  # Add products
│   │   ├── products_list.php # Product management
│   │   └── ...
│   └── server/
│       └── server.php         # Admin authentication logic
├── css/                       # Stylesheets
├── js/                        # JavaScript files
├── product_images/            # Product photos
├── index.php                  # Customer homepage
├── store.php                  # Product catalog
├── cart.php                   # Shopping cart
├── checkout.php               # Checkout page
└── db.php                     # Database connection
```

---

## Notes & Important Information

### ⚠️ Security Warnings

**This is a demonstration project. Before deploying to production:**

1. ✅ Change all default passwords
2. ✅ Use secure password hashing (bcrypt/Argon2 instead of MD5)
3. ✅ Enable HTTPS/SSL
4. ✅ Add CSRF protection
5. ✅ Sanitize all user inputs
6. ✅ Use environment variables for sensitive data
7. ✅ Set strong MySQL root password
8. ✅ Restrict database access
9. ✅ Enable firewall rules
10. ✅ Regular security updates

### 💡 Development Tips

- **Live Reload**: Code changes are immediately reflected (no need to rebuild)
- **Database Persistence**: Data persists even after `docker compose down`
- **Fresh Start**: Use `docker compose down -v` to reset database
- **Logs**: Use `docker compose logs -f` to debug issues

### 🐛 Common Issues

**Issue**: "Port 8080 already in use"

```bash
# Solution: Change port in docker-compose.yml
ports:
  - "8081:80"  # Use 8081 instead
```

**Issue**: "Container name already in use"

```bash
# Solution: Remove old containers
docker rm -f onlineshop_db_advanced onlineshop_web_advanced
```

**Issue**: Database connection errors

```bash
# Solution: Check if database is healthy
docker compose ps
docker logs onlineshop_db_advanced
```

**Issue**: Permission errors

```bash
# Solution: Fix permissions
docker compose exec web chown -R www-data:www-data /var/www/html
```

---

## Traditional Installation (Without Docker)

<details>
<summary>Click to expand XAMPP/WAMP installation instructions</summary>

### Using XAMPP or WAMP

1. Install XAMPP or WAMPP.

2. Open XAMPP Control panel and start [apache] and [mysql].

3. Download project from github(https://github.com/PuneethReddyHC/online-shopping-system-with-advanced-admin-page.git)  
   OR follow gitbash commands:

   ```bash
   cd C:\\xampp\htdocs\
   git clone https://github.com/PuneethReddyHC/online-shopping-system-with-advanced-admin-page.git
   ```

4. Extract files in C:\\xampp\htdocs\.

5. Open link localhost/phpmyadmin

6. Click on new at side navbar.

7. Give database name as `onlineshop` and hit create button.

8. After creating database, click on import.

9. Browse the file in directory[online-shopping-system-with-advanced-admin-page/database/onlineshop.sql].

10. After importing successfully.

11. Open any browser and type http://localhost/online-shopping-system-with-advanced-admin-page-master.

12. First register and then login.

13. Admin login details: Email=admin@gmail.com or username=admin and Password=123456789.

</details>

---

## Technology Stack

- **Backend**: PHP 8.0
- **Database**: MySQL 8.0
- **Frontend**: HTML5, CSS3, JavaScript, jQuery
- **UI Framework**: Bootstrap, Material Design
- **Containerization**: Docker & Docker Compose
- **Web Server**: Apache 2.4

---

## If you like my project

Bye me Cup of coffee

## visit my other repository with different admin pages with below link

https://github.com/PuneethReddyHC/online-shopping-system-advanced

https://github.com/PuneethReddyHC/event-management

## If you like my project hit a star button

# Screenshots

![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/adduser.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/adminproductadd.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/manageuser.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/manageuseradmin.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/productlistadmin.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/productlist.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/cartpage.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/homepage.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/loginmodal.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/mainpage.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/productpage.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/productzoom.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/registermodal.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/searchfilter.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/searchpage.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/store.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/storepage.png)
![Image of adduser](https://github.com/PuneethReddyHC/online-shopping-with-advanced-admin-page/blob/master/screenshot/storepage1.png)

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
