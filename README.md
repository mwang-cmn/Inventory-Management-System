# Inventory-Management-System
Simple inventory management system for an agrovet
# Inventory Management System

## **Project Overview**
This project is a full-stack Inventory Management System designed for a small business . It provides web and mobile interface to record sales, monitor inventory, track revenue and profit margins, and analyze business performance. The system features role-based access control for admins and sales attendants, and integrates real-time stock alerts to prevent stockouts.

---

## **Features**

### **Web Interface**
- Admin Dashboard:
  - View daily/monthly sales trends.
  - Monitor revenue, profit margins, and discrepancies between sales and inventory.
  - Manage inventory (add/edit/delete products and monitor stock levels).
  - Set and receive low-stock alerts.

### **Mobile App**
- Sales Attendant Functions:
  - Record transactions in real-time.
  - Check product availability and pricing.
  - View alerts for low-stock products.

- Admin Functions:
  - Monitor activities remotely.

### **Security**
- Role-Based Access Control:
  - Admin privileges to manage the system.
  - Restricted access for sales attendants.
- Secure user authentication using JWT.

### **Analytics**
- Visualized dashboards for sales and inventory.
- Automated alerts for stock replenishment.

---

## **Tech Stack**

### **Frontend**
- Web: React.js
- Mobile: React Native or Flutter
- Styling: Tailwind CSS or Material-UI

### **Backend**
- Node.js with Express.js

### **Database**
- PostgreSQL (centralized storage)

### **Hosting**
- Render/Vercel/Netlify for web.
- Railway for backend and database.

---

## **System Architecture**
1. **Frontend**:
   - Web and mobile apps communicate with the backend via REST APIs.
2. **Backend**:
   - API handles user authentication, role management, and business logic.
3. **Database**:
   - PostgreSQL stores user data, inventory details, sales records, and analytics.
4. **Notifications**:
   - Push notifications for stock alerts using Firebase or a similar service.

---

## **Database Schema**

### **Tables**:
- **Users**:
  - `id` (PK), `username`, `password`, `role` (admin or attendant)
- **Products**:
  - `id` (PK), `name`, `category`, `price`, `current_stock`, `reorder_level`
- **Sales**:
  - `id` (PK), `product_id` (FK), `quantity_sold`, `total_price`, `date`
- **Stock_Alerts**:
  - `id` (PK), `product_id` (FK), `alert_status` (triggered/not triggered)

---

## **Project Timeline**

### **Phase 1: Design and Planning (Weeks 1-2)**
- Create wireframes and UI/UX designs.
- Define system architecture and database schema.

### **Phase 2: Development (Weeks 3-6)**
- Build the backend API.
- Develop web and mobile interfaces.
- Implement authentication and role-based access.

### **Phase 3: Testing and Deployment (Weeks 7-8)**
- Test functionalities and fix bugs.
- Deploy the system using free hosting services.

---

## **Getting Started**

### **Prerequisites**
- Node.js
- PostgreSQL
- Git

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/inventory-management-system.git
   ```
2. Install dependencies for the backend and frontend:
   ```bash
   cd backend
   npm install
   ```
3. Set up the PostgreSQL database using the provided schema.
4. Start the backend server:
   ```bash
   npm start
   ```
5. Run the frontend:
   ```bash
   cd ../frontend
   npm start
   ```

---

## **Contributing**
- Fork the repository.
- Create a feature branch.
- Submit a pull request with a clear description of the feature or fix.

---
