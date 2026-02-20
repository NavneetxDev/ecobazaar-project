<div align="center">

# 🌿 EcoBazaar

### Your Gateway to Sustainable Shopping

*A modern full-stack marketplace built for environmentally conscious consumers and eco-friendly sellers*

[![Java](https://img.shields.io/badge/Java-17+-orange.svg)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![React](https://img.shields.io/badge/React-18-blue.svg)](https://reactjs.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

[Features](#features) • [Quick Start](#quick-start) • [Documentation](#project-documentation) • [Contributing](#contributing)

</div>

---

## 📖 About The Project

EcoBazaar is an innovative e-commerce solution designed to bridge the gap between sustainability and online shopping. Our platform exclusively features eco-friendly products, empowering users to make environmentally responsible purchasing decisions without compromise.

**What sets us apart:**
- Curated marketplace focused solely on sustainable products
- Transparency through eco-certification displays
- Community-driven approach to environmental responsibility
- Modern tech stack ensuring scalability and performance

## 🎯 Features

**Authentication & User Management**
- Secure user registration with email verification
- JWT-based authentication system
- Role-based access control (Admin, Seller, Customer)
- Personalized user profiles and dashboards

**Development Pipeline** (Coming Soon)
- Multi-vendor product listings with sustainability ratings
- Intelligent search with eco-filters
- Real-time shopping cart management
- Streamlined checkout with multiple payment options
- Order tracking and history
- Review and rating system
- Seller analytics dashboard
- Admin control panel for platform management

## 💻 Tech Stack

<table>
<tr>
<td valign="top" width="50%">

**Backend Infrastructure**

- **Framework:** Spring Boot 3.x
- **Language:** Java 17+
- **Database:** MySQL 8.0
- **Security:** Spring Security + JWT
- **ORM:** Spring Data JPA with Hibernate
- **Password Hashing:** BCrypt
- **Build:** Maven 3.6+
- **API Design:** RESTful architecture

</td>
<td valign="top" width="50%">

**Frontend Stack**

- **Library:** React 18
- **Build Tool:** Vite
- **Routing:** React Router v6
- **Styling:** CSS3 with modern practices
- **Code Quality:** ESLint
- **Package Manager:** npm/yarn
- **Development Server:** Vite Dev Server

</td>
</tr>
</table>

## 🚦 Quick Start

### System Requirements

Ensure you have the following installed on your machine:

```
✓ Java Development Kit (JDK) 17 or higher
✓ Maven 3.6+
✓ MySQL 8.0+
✓ Node.js 16.x or later
✓ npm or yarn package manager
```

### Installation Guide

**Step 1: Clone and Navigate**
```bash
git clone <your-repository-url>
cd Ecobazaar-Group-main
```

**Step 2: Configure Database**

Create a new MySQL database:
```sql
CREATE DATABASE ecobazaar CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

**Step 3: Launch Backend Server**

```bash
# Navigate to backend directory
cd ecobazaar

# Configure your database credentials
# Edit: src/main/resources/application.properties
# Update: spring.datasource.username and spring.datasource.password

# Build the project
./mvnw clean install

# Start the Spring Boot application
./mvnw spring-boot:run
```

Your backend API will be running at `http://localhost:8080`

**Step 4: Launch Frontend Application**

Open a new terminal window:

```bash
# Navigate to frontend directory
cd ecobazaar-frontend

# Install all dependencies
npm install

# Start development server
npm run dev
```

Access the application at `http://localhost:5173`

## 📂 Project Documentation

### Directory Overview

The project follows a modular architecture with clear separation of concerns:

**Backend Module** (`/ecobazaar`)
```
src/main/java/com/infosys/springboard/ecobazaar/
│
├── config/         → Application and security configurations
├── controller/     → REST API endpoint handlers
├── entity/         → Database entity models
├── repository/     → Data access layer interfaces
├── security/       → JWT utilities and security filters
├── service/        → Business logic implementation
└── EcoBazaarApplication.java
```

**Frontend Module** (`/ecobazaar-frontend`)
```
src/
│
├── components/     → Reusable UI components
├── features/       → Feature-specific modules
│   ├── admin/     → Admin dashboard components
│   ├── cart/      → Shopping cart functionality
│   ├── orders/    → Order management
│   ├── products/  → Product catalog
│   └── seller/    → Seller dashboard
├── pages/         → Route-level page components
├── services/      → API integration services
└── utils/         → Helper functions and constants
```

### API Reference

**Authentication Endpoints**

| HTTP Method | Endpoint | Request Body | Response | Description |
|-------------|----------|--------------|----------|-------------|
| POST | `/auth/register` | User details (JSON) | User object + JWT | Creates new user account |
| POST | `/auth/login` | Credentials (JSON) | JWT token | Authenticates user and returns token |

> Additional API endpoints are under active development and will be documented as they become available.

## 🗺️ Development Roadmap

**Current Status: Phase 1 - Foundation**

- [x] Initial project scaffolding
- [x] Backend API architecture
- [x] Frontend application setup
- [x] User authentication flow
- [x] Database schema design
- [x] Basic UI components

**Upcoming Milestones**

**Phase 2: Core Marketplace**
- [ ] Product CRUD operations
- [ ] Category management
- [ ] Shopping cart implementation
- [ ] Checkout workflow

**Phase 3: Payment & Orders**
- [ ] Payment gateway integration
- [ ] Order processing system
- [ ] Email notifications
- [ ] Invoice generation

**Phase 4: Community Features**
- [ ] Product reviews and ratings
- [ ] Wishlist functionality
- [ ] User recommendations
- [ ] Social sharing

**Phase 5: Sustainability Focus**
- [ ] Eco-score calculation algorithm
- [ ] Carbon footprint tracking
- [ ] Certification verification system
- [ ] Green shipping options

**Phase 6: Platform Management**
- [ ] Comprehensive admin dashboard
- [ ] Seller onboarding and management
- [ ] Advanced analytics and reporting
- [ ] Inventory management system

## ⚠️ Current Limitations

This project is in active development. Known areas for improvement include:

- Frontend-backend authentication integration requires refinement
- Enhanced error handling across API endpoints needed
- Client-side form validation enhancement in progress
- Testing coverage expansion underway

## 🤝 Contributing

We welcome contributions from the community! Whether you're fixing bugs, improving documentation, or proposing new features, your input is valued.

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 💬 Contact & Support

Have questions or need assistance? Feel free to open an issue in the repository.

---

<div align="center">

**Built with ❤️ for a sustainable future**

*EcoBazaar - Where Every Purchase Counts* 🌍

</div>
