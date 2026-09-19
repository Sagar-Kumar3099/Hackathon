# ♻️ Textile Waste Collection & Route Optimization Platform

A full-stack platform designed to connect **textile factories, waste collectors, and recyclers** in a digital marketplace where textile waste can be listed, purchased, collected, and routed efficiently for recycling and reuse.

## 🚀 Live Demo

🔗 **Live Application:**
https://imaginative-exploration-production-ac45.up.railway.app/

---

## 📌 About the Project

The textile industry generates a large amount of waste that can still be reused or recycled. However, factories may struggle to find suitable buyers, while recyclers may struggle to discover and collect recyclable textile materials.

This platform provides a centralized marketplace that connects both sides.

### 🏭 Textile Factories

Factories can:

* List their available textile waste
* Provide details about the waste material
* Specify quantity and other relevant information
* Make waste available for purchase by recyclers
* Manage their waste listings

### ♻️ Recyclers / Buyers

Recyclers can:

* Browse available textile waste
* Find suitable materials
* Purchase available waste
* Manage their orders
* Arrange collection of purchased materials

### 🚚 Collection & Route Optimization

The platform also focuses on the logistics involved in collecting textile waste.

Collection points and waste locations can be managed so that waste can be collected and transported efficiently.

---

## 🎯 Problem Statement

A significant amount of textile waste is generated during manufacturing and production.

Without an organized system:

```text
Textile Factory
       │
       ▼
    Waste
       │
       ▼
  Difficult to find
      buyers
       │
       ▼
   Waste may be
   underutilized
```

The platform creates a digital connection between waste generators and recyclers:

```text
                 ┌──────────────────┐
                 │ Textile Factory  │
                 └────────┬─────────┘
                          │
                    List Waste
                          │
                          ▼
                ┌─────────────────────┐
                │   Textile Waste     │
                │      Platform       │
                └──────────┬──────────┘
                           │
                    Match / Purchase
                           │
                           ▼
                  ┌─────────────────┐
                  │    Recycler     │
                  └────────┬────────┘
                           │
                       Collection
                           │
                           ▼
                  ┌─────────────────┐
                  │ Collection Point│
                  └────────┬────────┘
                           │
                     Optimized Route
                           │
                           ▼
                    ♻️ Recycling
```

---

## ✨ Key Features

### 🏭 Waste Listing

Factories can create listings for textile waste and make them available to potential buyers.

Information can include:

* Waste/material type
* Quantity
* Location
* Description
* Availability
* Other relevant material details

---

### ♻️ Waste Marketplace

The platform acts as a marketplace connecting:

```text
Waste Generators  ↔  Platform  ↔  Recyclers
```

Factories can offer waste while recyclers can discover materials that are suitable for their recycling requirements.

---

### 🔎 Material Discovery

Recyclers can browse available textile materials and identify waste that matches their requirements.

This helps reduce the gap between:

**"I have textile waste"**

and

**"I need textile waste for recycling."**

---

### 🛒 Waste Purchase

Recyclers can purchase available textile waste from factories through the platform.

The system can maintain information about:

* Buyer
* Seller
* Material
* Quantity
* Order
* Collection status

---

### 📦 Order Management

The platform keeps track of waste purchase/order information so that the lifecycle of a transaction can be managed.

```text
Waste Listed
     ↓
Available
     ↓
Purchased
     ↓
Collection
     ↓
Collected
     ↓
Recycled / Reused
```

---

### 📍 Collection Points

The platform supports collection-point management to help organize where textile waste can be collected and consolidated.

This can help reduce unnecessary transportation and make collection operations easier to manage.

---

### 🚚 Route Optimization

One of the key aspects of the project is optimizing the route used to collect textile waste.

Instead of collecting materials through inefficient routes:

```text
Factory A ────────┐
                  │
Factory B ────────┼──► Collection
                  │
Factory C ────────┘
```

The platform can organize collection locations and routes to improve transportation efficiency.

---

## 🔄 Complete Workflow

### Step 1 — Factory Lists Waste

```text
Factory
   ↓
Create Waste Listing
   ↓
Add Material Details
   ↓
Specify Quantity & Location
```

### Step 2 — Recycler Finds Waste

```text
Recycler
   ↓
Browse Available Materials
   ↓
Find Required Textile Waste
   ↓
View Listing
```

### Step 3 — Purchase

```text
Recycler
   ↓
Purchase Waste
   ↓
Order Created
```

### Step 4 — Collection

```text
Purchased Waste
       ↓
Collection Planning
       ↓
Collection Point
```

### Step 5 — Transportation

```text
Collection Locations
       ↓
Route Optimization
       ↓
Efficient Transportation
       ↓
Recycler
```

### Step 6 — Recycling / Reuse

```text
Recycler
   ↓
Process Textile Waste
   ↓
♻️ Recycle / Reuse
```

---

## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │       Users         │
                    │                     │
                    │ Factory / Recycler  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Web Frontend     │
                    │                     │
                    │   React / Vite      │
                    └──────────┬──────────┘
                               │
                         HTTP / REST
                               │
                               ▼
                    ┌─────────────────────┐
                    │      Backend        │
                    │                     │
                    │ Node.js / Express   │
                    └──────────┬──────────┘
                               │
                 ┌─────────────┴─────────────┐
                 │                           │
                 ▼                           ▼
        ┌─────────────────┐        ┌─────────────────┐
        │    Database     │        │ Business Logic  │
        │                 │        │                 │
        │    MongoDB      │        │ Matching        │
        └─────────────────┘        │ Orders          │
                                   │ Collection      │
                                   │ Routing         │
                                   └─────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Vite
* JavaScript
* HTML
* CSS
* Lucide React

### Backend

* Node.js
* Express.js
* REST APIs

### Database

* MongoDB
* MongoDB Atlas

### Deployment

* Railway
* GitHub

---

## 📂 Major Modules

The application is organized around several core modules:

```text
Authentication
      │
      ├── User Management
      │
      ├── Textile Materials
      │
      ├── Waste Collection
      │
      ├── Collection Points
      │
      ├── Orders
      │
      ├── Matching
      │
      ├── Vendors
      │
      ├── Disposal
      │
      └── Route / Logistics
```

---

## 🔐 Authentication

The platform provides authentication functionality for users so that different users can interact with the system based on their role.

Possible user types include:

* Textile factories
* Recyclers
* Collection partners
* Vendors

---

## 🔗 API Architecture

The backend follows a REST API architecture.

Major API areas include:

```text
/api/auth
/api/material
/api/order
/api/matching
/api/collection-point
/api/disposal
/api/reuse
/api/textile
/api/vendor
```

These APIs handle communication between the frontend and backend services.

---

## 🗄️ Database

MongoDB is used to store application data.

The platform manages data related to:

* Users
* Textile materials
* Waste listings
* Orders
* Collection points
* Vendors
* Matching
* Disposal
* Reuse
* Collection activities

---

## 🔄 Buyer-Seller Matching

The matching functionality helps connect textile waste with potential buyers.

Conceptually:

```text
Factory
   │
   │ Material Type
   │ Quantity
   │ Location
   ▼
Matching System
   │
   ▼
Potential Recycler
   │
   ▼
Purchase
```

This helps recyclers discover materials that match their requirements.

---

## 🌱 Sustainability Goal

The project supports the concept of a **circular textile economy** by making it easier to move textile waste from waste generators to organizations that can recycle or reuse it.

```text
Production
    ↓
Textile Waste
    ↓
Marketplace
    ↓
Recycler
    ↓
Recycling / Reuse
    ↓
New Value
```

Instead of treating textile waste as the end of a product lifecycle, the platform attempts to connect that waste with another useful lifecycle.

---

## ☁️ Deployment

The application is deployed on Railway.

### Production Flow

```text
GitHub
   │
   ▼
Railway
   │
   ├── Frontend
   │
   └── Backend
          │
          ▼
      MongoDB Atlas
```

### Live Application

**https://imaginative-exploration-production-ac45.up.railway.app/**

---

## 🚀 Running Locally

### Prerequisites

Make sure you have:

* Node.js
* npm
* MongoDB / MongoDB Atlas
* Git

---

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Hackathon
```

---

### 2. Install Dependencies

Install the project dependencies:

```bash
npm install
```

If frontend and backend have separate package files, install dependencies inside their respective directories as well.

---

### 3. Configure Environment Variables

Create a `.env` file and configure the required environment variables.

Example:

```env
MONGODB_URI=your_mongodb_connection_string
PORT=8080
FRONTEND_URL=http://localhost:5173
```

Do not commit `.env` or database credentials to GitHub.

---

### 4. Start the Backend

```bash
cd backend
node server.js
```

The backend will start on the configured port.

---

### 5. Start the Frontend

From the frontend directory:

```bash
npm run dev
```

The Vite development server will provide the local frontend URL.

---

## 📱 Responsive Design

The platform is designed to work across different screen sizes, including:

* Desktop
* Laptop
* Tablet
* Mobile

The interface adapts to smaller screens so users can access the platform from different devices.

---

## 🔮 Future Improvements

Potential improvements include:

* 🗺️ Real-time map integration
* 🚚 Advanced vehicle routing
* 📍 GPS-based collection tracking
* 📦 Real-time order tracking
* 💳 Online payment integration
* 📧 Email notifications
* 🔔 Push notifications
* ⭐ Factory/recycler ratings
* 📊 Advanced analytics dashboard
* 📈 Waste price prediction
* 🤖 AI-based material matching
* 📱 Dedicated mobile application
* 🔐 More granular role-based access control

---

## 🧠 Key Learning Outcomes

Through this project, I worked with:

* Full-stack application development
* React.js and Vite
* Node.js and Express.js
* REST API development
* MongoDB and MongoDB Atlas
* Authentication
* CRUD operations
* Marketplace workflows
* Buyer-seller matching
* Order management
* Collection-point management
* Logistics and route optimization concepts
* API integration
* Environment variable management
* Production deployment using Railway
* Debugging deployment and CORS-related issues

---

## 🌍 Project Impact

The goal of this platform is to make textile waste more **discoverable, tradable, collectible, and reusable**.

```text
             ┌──────────────┐
             │    Factory   │
             └──────┬───────┘
                    │
              Textile Waste
                    │
                    ▼
          ┌──────────────────┐
          │     Platform     │
          └────────┬─────────┘
                   │
              Marketplace
                   │
                   ▼
          ┌──────────────────┐
          │     Recycler     │
          └────────┬─────────┘
                   │
              Collection
                   │
                   ▼
          ┌──────────────────┐
          │ Recycling/Reuse  │
          └──────────────────┘
```

---

## 👨‍💻 Author

**Sagar Kumar**

Full Stack / Backend Developer

### Interests

* Node.js
* Express.js
* NestJS
* React.js
* TypeScript
* MongoDB
* PostgreSQL
* REST APIs
* Backend Development

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

### 🔗 Live Demo

https://imaginative-exploration-production-ac45.up.railway.app/
