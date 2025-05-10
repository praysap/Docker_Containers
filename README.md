# Microservices Task – Dockerized Node.js Services

This project demonstrates a basic microservices architecture using **Node.js**, **Docker**, and **Docker Compose**. It includes the following services:

- **User Service** – Runs on port `3000`
- **Product Service** – Runs on port `3001`
- **Order Service** – Runs on port `3002`
- **Gateway Service** – Runs on port `3003` (acts as an API aggregator)

---

## 📁 Project Structure
---
submission/
├── user-service/
│ ├── Dockerfile
│ └── index.js
├── product-service/
│ ├── Dockerfile
│ └── index.js
├── order-service/
│ ├── Dockerfile
│ └── index.js
├── gateway-service/
│ ├── Dockerfile
│ └── index.js
├── docker-compose.yml
└── README.md

---
## Services and Endpoints 192.168.1.34

### **User Service**
- **Base URL:** `http://192.168.1.34:3000`
- **Endpoints:**
  - **List Users:**  
    ```
    curl http://192.168.1.34:3000/users
    ```
    Or open in your browser: [http://192.168.1.34:3000/users](http://192.168.1.34:3000/users)

    <img width="501" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/users.png" />


---

### **Product Service**
- **Base URL:** `http://192.168.1.34:3001`
- **Endpoints:**
  - **List Products:**  
    ```
    curl http://192.168.1.34:3001/products
    ```
    Or open in your browser: [http://192.168.1.34:3001/products](http://192.168.1.34:3001/products)

    <img width="455" alt="image" src="https://github.com/Docker_Containers/blob/main/assets/8fd78e2a-66b1-4751-8790-5b95b52bb808" />


---

### **Order Service**
- **Base URL:** `http://192.168.1.34:3002`
- **Endpoints:**
  - **List Orders:**  
    ```
    curl http://192.168.1.34:3002/orders
    ```
    Or open in your browser: [http://192.168.1.34:3002/orders](http://192.168.1.34:3002/orders)

    <img width="430" alt="image" src="https://github.com/Docker_Containers/blob/main/assets/fce958d2-e20d-44bc-9a7f-b9b24c0393a4" />


---

### **Gateway Service**
- **Base URL:** `http://192.168.1.34:3003/api`
- **Endpoints:**
  - **Users:**  
    ```
    curl http://192.168.1.34:3003/api/users
    ```
<img width="427" alt="image" src="https://github.com/Docker_Containers/blob/main/assets/b1122566-0041-40ac-bfa6-8c9faf705ea3" />

    
  - **Products:**  
    ```
    curl http://192.168.1.34:3003/api/products
    ```
<img width="417" alt="image" src="https://github.com/Docker_Containers/blob/main/assets/537a55a4-8ac2-4d2f-94ec-5246a2695069" />

    
  - **Orders:**  
    ```
    curl http://192.168.1.34:3003/api/orders
    ```
<img width="352" alt="image" src="https://github.com/Docker_Containers/blob/main/assets/18392da4-1d2c-4d6c-b257-0e034de2408a" />



---

## Instructions
1. Start all services using the `docker-compose` file:
   ```
   docker-compose up
   ```
<img width="854" alt="image" src="https://github.com/Docker_Containers/blob/main/assets/d25f9129-5514-430a-b836-ebc544a573c7" />
<img width="268" alt="image" src="https://github.com/Docker_Containers/blob/main/assets/2b49c94a-1dd3-4f1a-bdd0-04a10c1921ac" />


2. Once the services are running, use the above endpoints to verify the functionality.

Happy testing!
