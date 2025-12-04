# Hotel-Management-System
Hotel Room Booking Project

# Hotel Management System — README.md

A simple PHP-based Hotel Management System built for learning and academic purposes. It includes customer registration, reservation creation, booking management, and an admin dashboard. The project uses PHP, MySQL, HTML/CSS, and JavaScript, and follows a minimal MVC-like structure.

> **Note:** This project is educational and may contain non-optimized or insecure code, as acknowledged in the original documentation. Not intended for production use.

---

## 📌 Features

### Customer Features
- Create an account and log in  
- View available room types  
- Make a reservation (select dates, room type, requirements, adults/children, additional notes)
- View booking status (PENDING / CONFIRMED / CANCELLED)
- Update personal information  

### Admin Features
- Manage all reservations (approve, cancel)
- View customers and their bookings
- Update customer roles (convert a customer to admin)

---

## 🗂️ Project Structure

| Component | Description |
|----------|-------------|
| `index.php` | Home page / entry point of the application |
| `sign-in.php` | User login system |
| `customer/` | Customer pages such as viewing bookings |
| `admin/` | Admin dashboard for reservation management |
| **Database** | Tables: `customer`, `reservation`, `booking` |

---

## 🛢️ Database Setup

1. Create a new database named **`hotel`**  
2. Import the provided `hotel.sql` file to create all tables and sample data:  
   ```sql
   mysql -u root -p hotel < hotel.sql
   ```
3. Ensure database credentials match your configuration in PHP (e.g., DB.php).

---

## ⚙️ Installation & Setup

1. Install **XAMPP**, **MAMP**, or any PHP + MySQL server.  
2. Place the project folder inside:
   - Windows: `xampp/htdocs/`
   - macOS: `Applications/MAMP/htdocs/`
3. Install JavaScript dependencies:
   ```bash
   npm install
   ```
4. Install PHP dependencies:
   ```bash
   composer install
   ```
5. Start Apache + MySQL.
6. Visit the project:
   ```
   http://localhost/hotel-mgmt-system/
   ```

---

## 👤 Creating an Account

1. Open:
   ```
   http://localhost/hotel-mgmt-system/register.php
   ```
2. To make an account an **admin**:
   - Open phpMyAdmin → `hotel` database  
   - Open `customer` table  
   - Set `isadmin = 1` for any user  

---

## 🧪 Developer Tools

Run PHPUnit tests:
```bash
./vendor/bin/phpunit tests
```

Run PHP Code Beautifier:
```bash
./vendor/bin/phpcbf app/*.php --standard=ruleset.xml
```

Run ESLint:
```bash
npm run eslint
npm run eslint -- --fix
```

---

## 📜 Code of Conduct

This project follows the Contributor Covenant Code of Conduct.  
Full text is included in `CODE_OF_CONDUCT.md`.

---

## 📄 License

See the included `LICENSE` file for usage terms.

---

## 🤝 Contributing

Issues and PRs are welcome. Please follow the Code of Conduct.

---

## 📬 Need Help?

Feel free to request:
- A more advanced README  
- ER diagrams  
- Setup instructions  
- UI redesign  
- API version  
