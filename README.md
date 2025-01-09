# Online Store Website

<p>
   An online store is a website or digital platform where businesses sell products or services to customers over the internet. It allows users to browse items, 
   add them to a virtual shopping cart, make secure payments, 
   and receive the goods or services through delivery or online access.
</p>

<p>
	The primary goal of an online store is to facilitate commercial transactions online. It bridges the gap between businesses 
	and customers by offering an 
	interactive platform where users can explore offerings, make purchases, and provide feedback.
</p> 

<p>
	It’s essentially a digital version of a physical shop, accessible 24/7, designed for convenience and a wide reach.
</p>

<p>For Online Demo : <a target="_blank" href="https://online-store-demo-sandyblades-projects.vercel.app/">https://online-store-demo-sandyblades-projects.vercel.app</a></p>

# Preview

<img src="https://i.ibb.co.com/YNQcQ4D/home.png" alt="home" />


# Features

<ol type="1">
	<li>
		Authentication
		<ol type="1">
			<li>Login</li>
			<li>Register</li>
			<li>Account Confirmation</li>
			<li>Forgot Password</li>
			<li>Reset Password</li>
		</ol>
	</li>
	<li>
		User Account
		<ol type="1">
			<li>Change Password</li>
			<li>Manage Profile</li>
		</ol>
	</li>
	<li>
		General Page
		<ol type="1">
			<li>Home</li>
			<li>Product Catalog</li>
			<li>Product Detail Page</li>
			<li>Shopping Cart</li>
			<li>Checkout Process</li>
			<li>Newslettter</li>
		</ol>
	</li>
</ol>

# Technologies Used

<ol type="1">
	<li>Visual Studio Code</li>
	<li>Modern Web Browser</li>
	<li>Git 2.4</li>
	<li>
		Backend Technologies
		<ol type="1">
			<li>MySQL 5.7 / Maria DB 11.3</li>
			<li>PHP 8.3</li>
			<li>Composer 2.7</li>
			<li>Symfony 6.4.x for REST API </li>
		</ol>
	</li>
	<li>
		Frontend Technologies
		<ol type="1">
			<li>CSS3</li>
			<li>HTML5</li>
			<li>Bootstrap 5</li>
			<li>Node JS LTS</li>
			<li>Vue 3</li>
		</ol>
	</li>
</ol>

## Getting Started
#### 1. Clone the repository and navigate to the directory
```shell
git clone https://github.com/sandyblade/symfony-online-store.git
cd symfony-online-store
```

#### 2. Install backend dependencies, please move to directory symfony-online-store/backend
```shell
composer install
```

#### 3. Make a .env.local file and customize its settings 
```shell
APP_TIMEZONE=UTC
DATABASE_URL="mysql://[DB_USER]:[DB_NAME]@[DB_HOST]:[DB_PORT]/[DB_NAME]?serverVersion=5.7"
```

#### 4. Start MySQL / Maria DB Service , Seed data and Running REST API
```shell

sudo service mysqld start / sudo systemctl start mariadb
CREATE DATABASE {database-name}

mkdir config/jwt

openssl genrsa -out config/jwt/private.pem 4096
openssl rsa -pubout -in config/jwt/private.pem -out config/jwt/public.pem

php bin/console lexik:jwt:generate-keypair
php bin/console doctrine:migrations:migrate
php bin/console doctrine:fixtures:load
php -S 0.0.0.0:8000 -t public
```

#### 5. Install frontend dependencies, please move to directory symfony-online-store/frontend
```shell
npm install
```

#### 6. Make a .env.local file and customize its settings 
```shell
VUE_APP_TITLE="My Store"
VUE_APP_AUTHOR="John Doe"
VUE_APP_DESCRIPTION="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book."
VUE_APP_BACKEND_URL="http://localhost:8000"
```

#### 7. Run Application 
```shell
cd frontend
npm run dev
```

#### 8. Access application by entering [https://localhost:5173](https://localhost:5173) in the browser.

<br/>
<img src="https://i.ibb.co.com/59584Rp/store.png" alt="store" />
</br>
<img src="https://i.ibb.co.com/CPM5Xb6/product.png" alt="product" />
</br>
<img src="https://i.ibb.co.com/GxN6Pg1/checkout.png" alt="checkout" />
</br>
<img src="https://i.ibb.co.com/KjRRdgH/login.png" alt="login"/>
</br>
<img src="https://i.ibb.co.com/wpX8yrg/register.png" alt="register" />


#### 9. Developer Contact
<ul>
	<li>
		<strong>Whatsapp</strong> <a target="_blank" href="https://wa.me/628989218470">https://wa.me/628989218470</a>
	</li>
	<li>
		<strong>Telegram</strong> <a target="_blank" href="https://t.me/sandyblade">https://t.me/sandyblade</a>
	</li>
	<li>
		<strong>Gmail</strong> <a  href="mailto:sandy.andryanto.blade@gmail.com">sandy.andryanto.blade@gmail.com</a>
	</li>
</ul>