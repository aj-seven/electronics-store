<p align="center">
  <img src="store/static/assets/electronics-icon.png" height="128">
  <h2 align="center"><a> electronics store </a></h2>
  <p align="center">Electronic store based on django framework <p>
</p>

## :star: Highlights
- Product management (via admin route)
- Category management (via admin route)
- User management (via admin route)
- Shipping cart
- Checkout and payment
- Order management
- Search and filtering
- Product reviews and ratings
- Promotions and discounts
- Admin dashboard
- Responsive design and email notifications

## Demo

<img width="1679" height="885" alt="Screenshot_20251102_141009" src="https://github.com/user-attachments/assets/d1d7254f-0b05-49e9-b071-dde68352c10e" />

<details closed>
<summary>
<h4> More here </h4>
</summary>
  <img width="1679" height="885" alt="Screenshot_20251102_135441" src="https://github.com/user-attachments/assets/4400a1d4-a969-4830-b1c7-f6a7eff95508" />
  <img width="1679" height="885" alt="Screenshot_20251102_135348" src="https://github.com/user-attachments/assets/f12065ae-0a64-43f4-a0a1-c00cdd73bbd9" />
  <img width="1679" height="885" alt="Screenshot_20251102_141028" src="https://github.com/user-attachments/assets/a809e495-934f-4e6c-af12-e5f6fb3581e5" />
</details>

## Development

Clone the repository, install the dependencies and start the application

**_Code Setup_**
```bash

# Clone the repo
git clone https://github.com/aj-seven/electronics-store
cd electronics-store

# Create virtual environment
python -m venv venv

# Activate virtual environment
source venv/bin/activate

# For Windows
cd venv
cd Scripts
.\activate.bat

# Install Requirements
pip install -r requirements.txt

# Make necessary Migrations
python manage.py makemigrations
python manage.py migrate

# Create admin as superuser
python manage.py createsuperuser

# Enter the admin details to manage the users, groups products, orders, etc...
Example view:
Username (leave blank to use 'user'): admin
Email address: test@gmail.com
Password: 
Password (again): 
Superuser created successfully.


```

**_Routes_**
- Admin Routes
  - http://127.0.0.1:8000/admin/ - Login with admin credentials that previously created
  - http://127.0.0.1:8000/admin/auth/user/ - Manage Normal users
  - http://127.0.0.1:8000/admin/auth/group/ - Manage Groups for staff like to manage products list (having certain previlege only)
  - http://127.0.0.1:8000/admin/shop/product/ - Able to add products with stocks, discount, price, name, description, etc
  - http://127.0.0.1:8000/admin/shop/category/ - Able to add Categories to a Product
  - http://127.0.0.1:8000/admin/shop/cartitem/ - Mange Cart Items for a user
  - http://127.0.0.1:8000/admin/shop/orderitem/ - Manage Order Items that a user is placed
  - http://127.0.0.1:8000/admin/shop/order/ - Manage Order List of a user

- User Routes
  - http://127.0.0.1:8000/ - homepage
  - http://127.0.0.1:8000/accounts/login/ - login page
  - http://127.0.0.1:8000/signup/ - register page
  - http://127.0.0.1:8000/profile/ - profile
  - http://127.0.0.1:8000/password-change/ - for chaning password (can be manage under admin route for user specific too)
  - http://127.0.0.1:8000/cart/ - Cart list
  - http://127.0.0.1:8000/orders/ - Order History
  - http://127.0.0.1:8000/product/1/ - More about product details
  - http://127.0.0.1:8000/checkout/ - checkout and place order after selection
