# PROJECT PROPOSAL
## Vybe Cart
### A Full-Featured Online Shopping Platform (Inspired by Daraz)


## 1. Introduction

Vybe Cart is a web-based e-commerce platform developed using Laravel, designed to provide a complete online shopping experience for customers and a powerful management interface for administrators. The system is inspired by Daraz, one of the most prominent online marketplaces in Nepal, and is adapted to the academic context of a university project. The project aims to simulate a realistic e-commerce environment where users can browse products, search categories, add items to cart, place orders, review products, and manage their personal wishlist. From the system’s actual implementation, the project includes both customer-facing functionalities and administrative controls, making it a suitable model of a small to medium-sized online retail platform.

The project is not merely a static website; it contains real business logic and database design based on Laravel’s MVC architecture. Models such as User, Product, Category, Cart, Order, Review, and Wishlist demonstrate a data-driven architecture where customer actions are linked to persistent records in the database. Controllers such as PagesController, ProductController, CategoryController, OrderController, CartController, ReviewController, WishlistController, and DashboardController implement core functionality such as browsing, ordering, product management, stock updates, search, and dashboard analytics. This indicates that the system is designed to behave like a functional online store rather than a sample application.

The actual project features a modern frontend with responsive views, product categories, hero product sliders, customer reviews, and an admin dashboard. The application includes authentication, role-based access control, order tracking, and email notifications, which are integral parts of an operational e-commerce system. Therefore, Vybe Cart is positioned as a practical academic solution that addresses both user experience and administrative management in the context of digital commerce in Nepal.


## 2. Problem Statement

The online shopping sector in Nepal has been growing rapidly, but many users still face common challenges in e-commerce systems. These include complicated product discovery, lack of trust in order processing, limited product information, weak stock visibility, and poor customer support mechanisms. Consumers often need a platform that is simple, fast, and reliable for browsing products, comparing prices, placing orders, and tracking the status of their purchases. On the other hand, administrators often need robust tools to manage categories, products, users, orders, and business statistics from a centralized dashboard.

Many existing marketplaces, although popular, may not fully suit the needs of local academic projects or small-scale digital commerce systems. There is a need for a simplified but realistic retail platform that demonstrates the essential workflow of online selling: product management, customer interaction, cart operations, order processing, and admin oversight. Vybe Cart addresses this gap by offering a full-featured Laravel-based shopping system inspired by the Daraz structure but tailored to a realistic academic implementation.

The system solves these issues by providing product search, category-based browsing, cart management, order placement, purchase-based review functionality, and a powerful admin dashboard that tracks users, products, and order statuses. It also incorporates stock adjustments when orders are processed or cancelled, helping maintain realistic inventory logic. In this way, Vybe Cart reflects both the customer journey and the business-side operations of an online shopping platform.


## 3. Objectives

The objectives of this project are based on the actual modules and business logic implemented in the codebase. The main objectives are as follows:

1. To design and develop a complete e-commerce web application that supports browsing, searching, and purchasing products online.
2. To implement a user-friendly customer interface where users can view products, add items to cart, place orders, check order history, and manage a wishlist.
3. To create an admin panel for managing categories, products, user roles, and order states.
4. To implement role-based access so that only administrators can access management features while general users interact with the storefront.
5. To include review and rating functionality that allows users to submit feedback after purchase or general product interaction.
6. To integrate stock management logic so product inventory is decreased or restored based on order status changes.
7. To provide analytics and dashboard reporting for sales, users, and order statuses.
8. To build a secure Laravel application using authentication, validation, and middleware-based access control.
9. To provide a real-world e-commerce experience inspired by Daraz while keeping the scope appropriate for an academic project.


## 4. Methodology

### 4.1 Requirement Identification

#### 4.1.1 Study of Existing System / Literature Review

The project concept is influenced by existing online shopping systems such as Daraz Nepal, which provide a customer-friendly interface for product discovery, comparison, and transaction processing. Daraz represents a widely used and successful e-commerce model in Nepal, featuring categories, promotions, inventory, search, and user engagement. While this system is inspired by such platforms, the actual project in this workspace implements a simplified but functional version of the same core concepts.

The literature review therefore focuses on how modern e-commerce platforms organize product catalogs, category filters, cart and checkout flows, payment validation, admin monitoring, and customer communication. In the developed project, these features are implemented in a Laravel-based architecture using MVC design, relational database tables, and Blade-based views for frontend rendering.

#### 4.1.2 Requirement Analysis

The project requirements are clearly evidenced in the codebase and include both functional and non-functional requirements.

##### Functional Requirements: Customer Side

- User registration and login using Laravel authentication flow.
- Product browsing through the home page, category pages, and all-products page.
- Product search and search suggestions based on product and category names.
- Product detail view with description, price, offers, stock, and reviews.
- Add product to cart with quantity validation.
- Update cart quantity and remove products from the cart.
- Checkout flow for placing orders.
- Order placement with COD and eSewa-style payment handling logic.
- User order history and order cancellation.
- Wishlist functionality for saving preferred products.
- Product review and rating submission with one-review-per-user-per-product rule.
- Verified purchase tracking for reviews.

##### Functional Requirements: Admin Side

- Admin dashboard with key metrics and analytics.
- Add, update, and delete product categories.
- Add, update, and delete products with image upload support.
- View all orders and update their status (Pending, Processing, Delivered, Cancelled).
- Manage stock values automatically according to order transitions.
- View all users and update or delete accounts.
- Toggle user roles between admin and user.
- Admin-only access through middleware protection.

##### Non-Functional Requirements

- Secure and validated user input through Laravel validation rules.
- Role-based access control to prevent unauthorized admin operations.
- Responsive interface using Tailwind CSS and modern frontend components.
- Database integrity through foreign keys and unique constraints.
- Scalability through model-based architecture and Eloquent relationships.
- Availability of email notifications for order updates and new order actions.
- Maintainability through separate controllers, models, migrations, and Blade views.

### 4.2 Feasibility Study

#### Technical Feasibility

The project is technically feasible because it is built on Laravel 12, which provides a scalable MVC framework for web application development. The system uses Eloquent ORM for database operations, Blade templates for views, and Laravel’s built-in authentication system. The use of Vite and Tailwind CSS provides a modern frontend toolchain. The application uses database relationships and migrations to support product, user, order, cart, review, and wishlist operations. The project therefore demonstrates strong technical feasibility within the academic scope of a final-year web development project.

#### Operational Feasibility

The system is operationally feasible because it targets a practical user workflow: customer browsing, selection, ordering, and admin management. The platform supports regular online shopping tasks and manages them through a structured administrative dashboard. The existence of views such as welcome page, category pages, my cart, my orders, wishlist, and admin dashboard shows that the project is operationally aligned with real-world e-commerce usage.

#### Economic Feasibility

The project is economically feasible because it uses an open-source technology stack and local development environment tools. Laravel, PHP, Tailwind CSS, Vite, and SQLite/MySQL require minimal commercial licensing cost. The system does not depend on heavy enterprise systems or paid SaaS components, which makes it suitable for academic and small business deployment scenarios.

#### Schedule Feasibility

A realistic project schedule for this implementation is as follows:

| Phase | Duration | Details |
|---|---:|---|
| Requirement analysis | 1 week | System study, problem identification, feature mapping |
| Database and model design | 1 week | Tables, relationships, migrations, Eloquent models |
| Authentication and user roles | 1 week | Laravel auth, admin middleware, profile management |
| Product and category modules | 2 weeks | CRUD, image upload, catalog pages |
| Cart, wishlist, and review modules | 2 weeks | Quantity logic, wishlist feature, rating system |
| Order and payment flow | 2 weeks | Checkout, status processing, COD/eSewa logic |
| Admin dashboard and analytics | 1 week | KPI cards, charts, user monitoring |
| Testing and refinement | 1 week | Validation, bug fixing, responsiveness |
| Final documentation | 1 week | Proposal, report, presentation preparation |

This schedule is realistic for a final semester project because the modules are already aligned with the actual structure of the codebase.

### 4.3 High Level Design of System

#### System Architecture

The application follows a standard Laravel MVC architecture:

- Model layer: User, Product, Category, Cart, Order, Review, Wishlist
- View layer: Blade templates for customer pages and admin pages
- Controller layer: PagesController, DashboardController, ProductController, CategoryController, CartController, OrderController, ReviewController, UserController, WishlistController
- Middleware layer: isAdmin for access restriction
- Database layer: MySQL/SQLite database with migrations

The design ensures separation of concerns and makes the application modular, structured, and easy to maintain.

#### Working Mechanism / System Flow

1. A user visits the homepage and browses trending products or categories.
2. The user views product details, checks the stock, and reviews existing feedback.
3. The user adds items to the cart and adjusts quantity if needed.
4. The user proceeds to checkout and places an order.
5. The order is stored in the orders table with buyer and product details.
6. Admins review pending, processing, and delivered orders from the dashboard.
7. Admins update order status and stock is adjusted automatically depending on the state transition.
8. Customers view order history and cancellation status through personal pages.
9. Additional features such as wishlist and reviews enhance user engagement.

#### Key Algorithms and Business Logic

The project implements important business logic that reflects real e-commerce operations:

- Cart quantity adjustment: if the quantity in cart exceeds the remaining stock, the quantity is automatically reduced to available stock.
- Product filtering and sorting: products can be filtered by category and searched by name; sorting includes latest, price low-to-high, price high-to-low, and rating-based ordering.
- Stock management: inventory decreases when an order moves to Processing or Delivered, and returns when an order is reversed to Pending or Cancelled.
- Review validation: only one review per user per product is allowed, and purchase-based verification is tracked.
- Role management: admin middleware restricts sensitive routes, while the UserController toggles roles between admin and user.
- eSewa payment processing: checkout logic checks the payment response status and stores order information when the payment is complete.
- Search suggestion generation: the system offers suggestions for matching products and categories as the user types.

#### Use Case Description

The major actors in the system are:

- Customer: registers/login, views products, adds wishlist items, adds products to cart, places orders, tracks status, writes reviews.
- Admin: manages categories and products, sees dashboard statistics, updates orders, manages users, toggles roles.
- System: validates requests, updates database, sends email notifications, enforces middleware restrictions.

#### Database Design Overview

The database design is built using Laravel migrations. Major tables include:

- users: stores account information, password, remember token, email verification, and role.
- categories: stores product categories and category ordering.
- products: stores product name, description, price, stock, discounted price, image, and category reference.
- carts: stores user-product quantity mappings for temporary shopping cart records.
- orders: stores product purchase details including price, quantity, address, payment method, payment status, and order status.
- reviews: stores user ratings and comments for products, with unique per-user-per-product constraints.
- wishlists: stores product items saved by a user, with uniqueness constraints.
- password_reset_tokens and sessions: Laravel built-in authentication tables.

The important relationships are as follows:

- User has many carts, orders, reviews, and wishlists.
- Category has many products.
- Product belongs to Category and has many reviews and wishlist records.
- Cart belongs to User and Product.
- Order belongs to User and Product.
- Review belongs to User and Product.
- Wishlist belongs to User and Product.


## 5. Expected Outcome

The final system is expected to deliver a complete and functional online shopping experience for both customers and administrators. For the customer, the project will provide a trustworthy and easy-to-use e-commerce experience that includes product discovery, search, category navigation, cart management, order placement, wishlist management, and product review functionality. For the admin, the system will provide a dashboard equipped with business insights, product management tools, user management, and order processing capabilities.

The expected outcome of the project is a real-world, academically acceptable e-commerce solution that demonstrates understanding of modern web application architecture, database design, and business logic. It will serve as a strong foundation for further enhancement, including advanced payment gateways, coupon systems, shipping modules, and a more complete fulfillment process.


## 6. Tools and Technologies Used

The actual technologies used in the project are based on the workspace and dependency files. They include:

- PHP 8.2
- Laravel Framework 12
- Composer for dependency management
- MySQL and SQLite support through Laravel database configuration
- Blade templating engine
- Tailwind CSS
- Vite for frontend build and asset handling
- JavaScript and Axios for interactive user flows
- Laravel Breeze for authentication scaffolding
- Eloquent ORM for database operations and query logic
- HTML5 and CSS3 for responsive frontend design


## 7. References

[1] Daraz Nepal, “Daraz - Online Shopping in Nepal,” [Online]. Available: https://www.daraz.com.np/

[2] Laravel Team, “Laravel Documentation,” [Online]. Available: https://laravel.com/docs

[3] PHP Group, “PHP Manual,” [Online]. Available: https://www.php.net/manual/en/index.php

[4] Oracle, “MySQL 8.0 Reference Manual,” [Online]. Available: https://dev.mysql.com/doc/refman/8.0/en/

[5] Tailwind CSS, “Tailwind CSS Documentation,” [Online]. Available: https://tailwindcss.com/docs

[6] Vite, “Vite Documentation,” [Online]. Available: https://vite.dev/guide/


---

## Summary of Key Features Found in the Codebase

- Product home page with hero slider and featured/trending items
- Category-based browsing and product filtering
- Full product search and live search suggestions
- Product detail pages with price, stock, discounts, and reviews
- Shopping cart with quantity update and delete functionality
- Checkout and order placement flow
- COD and eSewa-style payment handling logic
- User order history and order cancellation
- Wishlist management
- Customer product reviews with rating system
- Verified purchase tracking in review data
- Admin dashboard with analytics and status cards
- CRUD for categories and products
- Inventory management during order status transitions
- User management and role toggling between admin and user
- Email notification support for order and status updates
- Middleware-based admin access control
- Laravel authentication and profile management
- Responsive frontend with Tailwind CSS and modern UI components


