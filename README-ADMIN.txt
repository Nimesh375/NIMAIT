NIMA IT SOLUTIONS — ADMIN PANEL
================================

This version includes a PHP + JSON admin backend designed for normal shared hosting / cPanel.

1. Upload the entire folder to your hosting public_html (or a subfolder).
2. Make sure the server supports PHP 8+.
3. Open: /admin/
4. Default login:
   Username: admin
   Password: Nima@2026!
5. BEFORE publishing publicly, change the password hash in api/config.php.
   Generate a new hash with:
   php -r "echo password_hash('YOUR_NEW_PASSWORD', PASSWORD_DEFAULT), PHP_EOL;"
6. Product changes are saved to api/data/products.json.
7. Uploaded product images are saved in images/uploads/.
8. Inquiries are saved to api/data/inquiries.json.
9. If your host blocks write access, give api/data/ and images/uploads/ write permission for the PHP process.

Admin features
--------------
- Dashboard stats
- Add / edit / delete products
- Product price, category, stock and featured status
- Product image upload
- Customer inquiry management
- Store phone / WhatsApp / email / location / announcement settings
- Public products page reads the live product catalogue

Security
--------
This is intentionally lightweight for shared hosting. Use HTTPS, keep the admin URL private, and change the default password before launch.
