# 🌾 Agri-Ecommerce

<div align="center">

### 🛒 Smart Agriculture Shopping Platform

**Explore • Compare • Add to Cart • Shop Agricultural Products**

A modern and responsive agricultural e-commerce web application built with **React, Material UI, and React Router**.

<br>

[![React](https://img.shields.io/badge/React-19.2.3-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://react.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Material UI](https://img.shields.io/badge/Material--UI-7.3.6-007FFF?style=for-the-badge&logo=mui&logoColor=white)](https://mui.com/)
[![React Router](https://img.shields.io/badge/React_Router-7.11.0-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white)](https://reactrouter.com/)
[![Create React App](https://img.shields.io/badge/Create_React_App-5.0.1-09D3AC?style=for-the-badge&logo=createreactapp&logoColor=white)](https://create-react-app.dev/)

<br>

**Repository:** [JAYASURYA-5/Agri-Ecommerce](https://github.com/JAYASURYA-5/Agri-Ecommerce)

</div>

---

## 🌱 About The Project

**Agri-Ecommerce** is a React-based online shopping platform designed specifically for agricultural products.

The application provides users with a simple and modern interface to explore agricultural products, search and filter products, view product information, add items to a shopping cart, modify quantities, and calculate the total order value.

The project uses **Material UI** to create a clean agriculture-focused design with green as the primary theme color and orange as an accent color.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🏠 **Home Page** | Agriculture-focused landing page with hero section and categories |
| 🛍️ **Product Listing** | Browse available agricultural products |
| 🔍 **Product Search** | Search products by name or description |
| 🗂️ **Category Filter** | Filter products according to their category |
| 🛒 **Shopping Cart** | Add and manage products in the cart |
| ➕➖ **Quantity Control** | Increase or decrease product quantities |
| 💰 **Price Calculation** | Automatically calculate item subtotals and total price |
| 📦 **Product Details** | View individual product information |
| 📱 **Responsive UI** | Designed for different screen sizes |
| 🎨 **Material UI** | Modern reusable interface components |

The repository's project analysis specifically identifies product filtering, cart management, navigation, product details, and multiple agriculture-related categories.

---

## 🌾 Product Categories

The home page currently highlights categories such as:

- 💊 **Medicines** — Crop disease treatments
- 🌱 **Fertilizers** — Plant nutrients
- 🍎 **Fruits** — Fresh agricultural produce
- 🥕 **Vegetables** — Fresh vegetables
- 🌾 **Seeds** — High-yield agricultural seeds

Each category can direct users toward the product browsing experience.

---

## 🧭 Application Flow

```text
                         🌾 Agri-Ecommerce
                                │
                                ▼
                         🏠 Home Page
                                │
                ┌───────────────┼───────────────┐
                ▼               ▼               ▼
           🛍️ Products      🌱 Categories     ℹ️ About
                │
                ▼
        🔍 Search & Filter
                │
                ▼
         📦 Product Details
                │
                ▼
          🛒 Add to Cart
                │
                ▼
         🛒 Shopping Cart
                │
          ┌─────┴─────┐
          ▼           ▼
      ➕ Quantity   ➖ Quantity
          │           │
          └─────┬─────┘
                ▼
        💰 Total Calculation
                │
                ▼
         ✅ Checkout Flow
```

---

## 🏗️ Application Architecture

```text
┌─────────────────────────────────────────┐
│              React Application          │
├─────────────────────────────────────────┤
│                                         │
│              App.js                     │
│        ┌────────┼────────┐              │
│        │        │        │              │
│        ▼        ▼        ▼              │
│      Home    Products   Cart             │
│        │        │        │              │
│        │        ▼        │              │
│        │   ProductList   │              │
│        │        │        │              │
│        │        ▼        │              │
│        │ ProductDetail   │              │
│        │                 │              │
│        └────────┬────────┘              │
│                 ▼                       │
│          Cart Context                   │
│                 │                       │
│                 ▼                       │
│        Global Cart State                │
│                                         │
└─────────────────────────────────────────┘
```

The application uses React routing, Material UI theming, and a cart context approach for managing cart-related state.

---

## 🖥️ Main Pages

### 🏠 Home

The home page introduces the platform with:

- Agriculture-themed hero section
- Welcome message
- **Shop Now** action
- Feature cards
- Product categories
- Navigation to product browsing

### 🛍️ Products

The product section provides:

- Product grid
- Search functionality
- Category filtering
- Product cards
- Add-to-cart functionality

### 📦 Product Details

The product details component is designed to display:

- Product image
- Product name
- Product information
- Product price
- Product quantity
- Add-to-cart action

### 🛒 Shopping Cart

The cart page provides:

- Added product list
- Product thumbnails
- Unit prices
- Quantity controls
- Item subtotal
- Remove product option
- Total price
- Continue shopping option
- Checkout action

The cart functionality includes operations such as `removeFromCart()`, `updateQuantity()`, and `getTotalPrice()`.

---

## 🔎 Product Search & Filtering

The product listing component supports:

```text
Search by Product Name
          │
          ▼
Search by Description
          │
          ▼
Select Category
          │
          ▼
Filter Products
          │
          ▼
Display Matching Products
```

If no product matches the selected filters, the application can display a **No Products Found** message.

---

## 💰 Cart Calculation

The application calculates the shopping cart total based on product price and quantity.

### Item Subtotal

```text
Item Subtotal = Product Price × Quantity
```

### Total Cart Value

```text
Total = Sum of All Item Subtotals
```

Example:

```text
Product A
₹500 × 2 = ₹1000

Product B
₹250 × 3 = ₹750

-------------------
Total = ₹1750
```

---

## 🛠️ Tech Stack

### Frontend

| Technology | Purpose |
|---|---|
| ⚛️ React 19 | Frontend application |
| 🟨 JavaScript | Application logic |
| 🎨 Material UI | UI components and design |
| 🧭 React Router DOM | Page navigation |
| 💅 Emotion | Styling solution used with MUI |
| 🔷 MUI Icons | Interface icons |
| ⚡ Create React App | Development/build environment |

The repository currently specifies React `19.2.3`, React Router DOM `7.11.0`, Material UI `7.3.6`, Emotion, MUI Icons, and `react-scripts` `5.0.1`.

---

## 📁 Project Structure

```text
Agri-Ecommerce/
│
├── public/
│   ├── index.html
│   ├── manifest.json
│   └── robots.txt
│
├── src/
│   │
│   ├── components/
│   │   ├── ProductList.js
│   │   ├── ProductDetail.js
│   │   └── Footer.js
│   │
│   ├── pages/
│   │   ├── Home.js
│   │   └── CartPage.js
│   │
│   ├── data/
│   │   └── products.js
│   │
│   ├── context/
│   │   └── CartContext.js
│   │
│   ├── App.js
│   ├── App.css
│   ├── index.js
│   └── index.css
│
├── .gitignore
├── package.json
├── package-lock.json
├── TODO.md
└── README.md
```

The repository currently contains `public`, `src`, package files, `TODO.md`, and the React application components/pages described above.

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/JAYASURYA-5/Agri-Ecommerce.git
```

### 2️⃣ Navigate to the Project

```bash
cd Agri-Ecommerce
```

### 3️⃣ Install Dependencies

```bash
npm install
```

### 4️⃣ Start the Development Server

```bash
npm start
```

The React development server will start locally.

---

## 📜 Available Commands

| Command | Description |
|---|---|
| `npm install` | Install project dependencies |
| `npm start` | Start development server |
| `npm test` | Run tests |
| `npm run build` | Create production build |

---

## 🎨 UI Design

The project follows an agriculture-inspired visual theme.

### Primary Design

🟢 **Green**  
Used as the primary agriculture-focused color.

### Accent Design

🟠 **Orange**  
Used as an additional highlight color.

### Typography

The application uses **Roboto** as part of its Material UI theme configuration.

---

## 📸 Screenshots

Add your application screenshots here to make the GitHub README more attractive.

```markdown
## 📸 Screenshots

### 🏠 Home Page

![Home Page](screenshots/home.png)

### 🛍️ Products Page

![Products Page](screenshots/products.png)

### 📦 Product Details

![Product Details](screenshots/product-details.png)

### 🛒 Shopping Cart

![Shopping Cart](screenshots/cart.png)
```

### Recommended Screenshot Folder

```text
screenshots/
├── home.png
├── products.png
├── product-details.png
└── cart.png
```

---

## 🎯 Project Objectives

The main objectives of the project are:

- 🌱 Create an online platform for agricultural products.
- 🛒 Provide a simple shopping experience.
- 🔍 Make product discovery easier through search and filters.
- 📦 Provide product information before purchasing.
- 💰 Automatically calculate shopping cart totals.
- 📱 Build a responsive and user-friendly interface.
- ⚛️ Practice modern React development.
- 🎨 Implement a reusable Material UI component system.

---

## 💡 What I Learned

This project helped develop practical knowledge in:

- React component development
- React state management
- React Context API
- React Router
- Material UI
- Responsive web design
- Product filtering
- Shopping cart implementation
- Dynamic price calculations
- Reusable UI components
- Git and GitHub workflow

---

## 🔮 Future Enhancements

The project can be extended with:

- 🔐 User registration and login
- 🗄️ Backend database integration
- 👨‍🌾 Farmer/seller dashboard
- 📦 Product management system
- 💳 Online payment gateway
- 🚚 Order tracking
- 📧 Email notifications
- ⭐ Product reviews and ratings
- ❤️ Wishlist functionality
- 📊 Admin dashboard
- 🔎 Advanced product filtering
- 📱 Mobile application
- ☁️ Cloud deployment
- 🤖 AI-based product recommendations

---

## 🌍 Real-World Use Case

The platform can be developed into a complete digital marketplace for agricultural products.

### 👨‍🌾 Farmers

Farmers can eventually use the platform to:

- List agricultural products
- Manage product information
- Update stock
- Receive customer orders
- Reach more customers

### 🛒 Customers

Customers can eventually:

- Discover agricultural products
- Compare products
- Add products to their cart
- Place orders
- Track deliveries
- Review products

---

## ⭐ Why This Project?

Traditional agricultural shopping can involve limited product availability and dependency on local markets.

An online agricultural marketplace can provide a more convenient digital experience by allowing customers to discover products online while creating opportunities for agricultural sellers to reach a wider audience.

---

## 👨‍💻 Developer

<div align="center">

### **Jayasurya K**

💻 Full Stack Developer | React Developer | Software Developer

🔗 **GitHub:**  
https://github.com/JAYASURYA-5

🌐 **Portfolio:**  
https://jayasurya6.netlify.app/

</div>

---

## ⭐ Support

If you like this project:

⭐ **Star this repository**

🍴 **Fork the repository**

🐛 **Report an issue**

💡 **Suggest new features**

---

<div align="center">

## 🌾 Agri-Ecommerce

### **Growing Agriculture Through Technology**

**Built with ❤️ using React**

</div>
