# E-Vendor-E-Commerce-Platform-with-Virtual-Wallet
E-Vendor is a simple yet powerful PHP-based e-commerce platform that integrates a virtual wallet system for managing payments, withdrawals, and commissions.
Built using PHP (MySQLi), JavaScript, HTML, and CSS, it provides a smooth shopping and wallet experience for users and a flexible structure for developers.

====Features====
===🧑‍💼 User Features==
  🔐 User Authentication: Secure login and registration system.
    🛒 Product Browsing & Purchase: View products, add to cart, and make purchases using wallet funds.
    💰 Virtual Wallet:
    Fund your wallet (e.g., via Paystack or manual deposit).
    View wallet balance in real time.
    Withdraw available funds easily.
    Automatic commission (2%) deducted during funding.
    📜 Transaction History: Track wallet funding, purchases, and withdrawals.
    📱 Responsive Interface: Works on both desktop and mobile browsers.

===🧑‍💻 Admin Features===
🧾 Manage products (add, edit, delete).
👥 Manage users and wallet balances.
💳 View and approve withdrawal requests.
📊 Generate transaction and user activity reports.

======🧱 Tech Stack=====
| Component           | Technology Used                     |
| ------------------- | ----------------------------------- |
| Backend             | PHP (MySQLi)                        |
| Frontend            | HTML5, CSS3, JavaScript             |
| Database            | MySQL                               |
| Payment Simulation  | Paystack (or manual funding option) |
| Server Requirements | Apache/Nginx, PHP 7.4+              |


=======📂 Folder Structure======
E-Vendor/
│
├── _includes/
│   └── dbconnect.php        # Database connection file
│
├── assets/
│   ├── css/                 # Stylesheets
│   ├── js/                  # JavaScript files
│   └── images/              # Product and user images
│
├── pages/
│   ├── login.php            # User login
│   ├── register.php         # User registration
│   ├── index.php            # Home/dashboard
│   ├── fund-wallet.php      # Fund wallet page
│   ├── withdraw.php         # Withdraw funds page
│   ├── initiate_fund.php    # Handles funding request logic
│   └── transactions.php     # View wallet transaction history
│
├── admin/
│   ├── dashboard.php        # Admin panel
│   ├── manage-products.php  # Product management
│   └── manage-users.php     # User management
│
└── README.md                # Project documentation

=====💳 Wallet Funding Example=====
Minimum deposit: ₦100
2% commission deducted automatically.
Net amount credited: 98% of the deposit.
Example:
If a user funds ₦1000 → ₦20 (2%) is deducted → ₦980 credited to wallet balance.

======🧠 How It Works=====
User logs in or registers.
Funds wallet → amount stored in wallet table.
Can purchase items from products table using wallet balance.
Withdraw requests logged in transactions table.
Admin can approve withdrawals or top-ups manually.

=====Database Tables (Simplified Overview)=====
| Table          | Description                            |
| -------------- | -------------------------------------- |
| `users`        | Stores user account details            |
| `wallet`       | Tracks each user’s wallet balance      |
| `transactions` | Stores all credit/debit records        |
| `products`     | Product catalog for e-commerce section |
| `orders`       | Records each user’s purchase           |

======🧰 Future Enhancements====
Integration with Paystack API for live payments.
Add product reviews and ratings.
Real-time wallet balance update using AJAX.
Optional mobile-friendly dashboard using Tailwind or Bootstrap.

======🧑‍🏫 Author=======
Name: Onyeacholem Ifeanyi Joshua
GitHub: @Gjeotech
Email: brandykoke@gmail.com

