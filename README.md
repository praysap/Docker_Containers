# Microservices Task – Dockerized Node.js Services

This project demonstrates a basic microservices architecture using **Node.js**, **Docker**, and **Docker Compose**. It includes the following services:

- **User Service** – Runs on port `3000`
- **Product Service** – Runs on port `3001`
- **Order Service** – Runs on port `3002`
- **Gateway Service** – Runs on port `3003` (acts as an API aggregator)

---

## 📁 Project Structure
```
Docker_Cotainers/
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
```
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

    <img width="501" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/project.png" />


---

### **Product Service**
- **Base URL:** `http://192.168.1.34:3001`
- **Endpoints:**
  - **List Products:**  
    ```
    curl http://192.168.1.34:3001/products
    ```
    Or open in your browser: [http://192.168.1.34:3001/products](http://192.168.1.34:3001/products)

    <img width="455" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/product.png" />


---

### **Order Service**
- **Base URL:** `http://192.168.1.34:3002`
- **Endpoints:**
  - **List Orders:**  
    ```
    curl http://192.168.1.34:3002/orders
    ```
    Or open in your browser: [http://192.168.1.34:3002/orders](http://192.168.1.34:3002/orders)

    <img width="430" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/orders.png" />


---

### **Gateway Service**
- **Base URL:** `http://192.168.1.34:3003/api`
- **Endpoints:**
  - **Users:**  
    ```
    curl http://192.168.1.34:3003/api/users
    ```
<img width="427" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/gateway_users.png" />

    
  - **Products:**  
    ```
    curl http://192.168.1.34:3003/api/products
    ```
<img width="417" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/gateway_products.png" />

    
  - **Orders:**  
    ```
    curl http://192.168.1.34:3003/api/orders
    ```
<img width="352" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/gateway_orders.png" />



---

## Instructions
1. Start all services using the `docker-compose` file:
   ```
   docker-compose up
   ```
<img width="854" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/Docker_up.png" />
<img width="268" alt="image" src="https://github.com/praysap/Docker_Containers/blob/main/assets/Docker_compose_up.png" />


2. Once the services are running, use the above endpoints to verify the functionality.

Happy testing!
