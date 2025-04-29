# 🛒 sb-ecom - E-Commerce REST API

A production-ready Spring Boot backend for an eCommerce platform. It supports user authentication, product management, shopping cart, orders, and user addresses.

---

## 🚀 Features

- 🧑 User authentication with JWT
- 📦 Product CRUD operations
- 🛒 Cart management
- 🧾 Order placement (if present)
- 🏠 User address management
- 🧱 Layered architecture (Controller → Service → Repository)

---

## 📂 Controllers Overview

### 🔐 AuthController
| Method | Endpoint               | Description              |
|--------|------------------------|--------------------------|
| POST   | `/api/auth/signin`     | Login                    |
| POST   | `/api/auth/signup`     | Register                 |
| GET    | `/api/auth/user`       | Get user details         |
| GET    | `/api/auth/username`   | Get logged in username   |
| POST   | `/api/auth/signout`    | Logout                   |

---

### 🛒 CartController
| Method | Endpoint                                              | Description                     |
|--------|-------------------------------------------------------|---------------------------------|
| POST   | `/api/carts/products/{productId}/quantity/{quantity}` | Add product to cart             |
| GET    | `/api/carts`                                          | View all carts                  |
| GET    | `/api/carts/users/cart`                               | View logged in user's cart      |
| PUT    | `/api/cart/products/{productId}/quantity/{operation}` | Update product quantity or remove |
| DELETE | `/api/carts/{cartId}/product/{productId}`             | Remove product from cart        |

---

### 🏠 AddressController
| Method | Endpoint                       | Description                 |
|--------|--------------------------------|-----------------------------|
| POST   | `/api/addresses`               | Create new address          |
| GET    | `/api/addresses`               | List all addresses          |
| GET    | `/api/addresses/{addressId}`   | Get address by ID           |
| GET    | `/api/users/addresses`         | Get addresses for logged in user |
| PUT    | `/api/addresses/{addressId}`   | Update address              |
| DELETE | `/api/addresses/{addressId}`   | Delete address              |

---

## ▶️ How to Run

```bash
git clone https://github.com/your-username/sb-ecom.git
cd sb-ecom
mvn spring-boot:run

[ecommerce-er-diagram.pdf](https://github.com/user-attachments/files/18275739/001.ecommerce-er-diagram.pdf)
![001 ecommerce-er-diagram-1](https://github.com/user-attachments/assets/be29a0a0-2060-46cd-a5b9-ab1d7cf49894)
![Image](https://github.com/user-attachments/assets/008afe41-2bf4-4cfa-832c-969ddd229f1e)

![Image](https://github.com/user-attachments/assets/bc325ae1-12f6-41ab-9af4-f17fe2b420d5)

![Image](https://github.com/user-attachments/assets/8bb9fdc3-e1f1-4ea4-986c-7316f9bf865e)

![Image](https://github.com/user-attachments/assets/a4da8bf6-f18b-48d2-a791-f3adf72239df)

![Image](https://github.com/user-attachments/assets/40ea28db-0a30-4c5e-8baf-54e281700f6c)

![Image](https://github.com/user-attachments/assets/9aac4174-f60b-4883-b069-426ad3e24cae)


