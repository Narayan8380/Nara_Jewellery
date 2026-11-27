Nara Jewellery

A premium gold jewellery showcase website built with Django. Customers browse collections, save favourites to a wishlist, and request a **free home visit**. There is no cart or online payment by design: payment happens in person, which protects customers from online fraud.

> Showroom: Marathahalli, Bangalore. Home visits across Bangalore.

Features
- User authentication: signup, login, logout, profile
- Product listing with category filters, search and pagination
- Wishlist with add/remove without page reload (AJAX with CSRF protection)
- Home-visit request form saved to the database and managed in Django admin
- Live gold rate from an external API, cached for 30 minutes, with a fallback value if the API is down
- WhatsApp enquiry links, custom 404 page, responsive Bootstrap 5 UI

Tech Stack
Python, Django, Bootstrap 5, HTML, CSS, JavaScript, SQLite

Run Locally
```bash
git clone https://github.com/Narayan8380/Nara_Jewellery.git
cd Nara_Jewellery
python -m venv .venv
.venv\Scripts\activate        # Windows
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```
Open http://127.0.0.1:8000/ and add products at /admin/.

Project Structure
- `products/` – products, categories, visit requests, gold rate service
- `users/` – signup, login, profile
- `wishlist/` – wishlist model and AJAX toggle
- `templates/`, `static/`, `media/` – UI, CSS and product images

Developer

Narayanamma Bojja

Project Type: Individual Project

