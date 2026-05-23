# Amazon-Profit-Tool-Demo

## Screenshots

![Dashboard](img1.jpeg)

![Profit Analysis](img2.jpeg)

![Order Report](img3.jpeg)

![Order Report](img4.jpeg)

![Order Report](img5.jpeg)

# Amazon Profit Analyzer

A full-stack business analytics application built to process Amazon seller reports and calculate accurate profit insights using Spring Boot and React.

---

## Features

- Upload Amazon Order Reports
- Upload Amazon Settlement Reports
- SKU-wise Cost Management
- Profit & Revenue Analytics
- JWT-based Authentication
- Dashboard for Business Insights

---

## Backend (Spring Boot)

The backend service processes Amazon reports and calculates:

- Total Revenue
- Total Cost (SKU-wise)
- Total Profit
- Profit Margin
- SKU-wise Profit Breakdown

### Tech Stack

- Java 17
- Spring Boot
- Spring Security (JWT)
- MySQL
- Hibernate / JPA
- Maven

---

## Frontend (React + Vite)

The frontend dashboard allows users to:

- Register & Login
- Upload CSV Reports
- Manage SKU Costs
- View Profit Analytics Dashboard

### Frontend Tech Stack

- React
- Vite
- Axios
- React Router
- Tailwind CSS

---

## Authentication APIs

| Endpoint | Method | Description |
|---|---|---|
| `/api/auth/register` | POST | Register User |
| `/api/auth/login` | POST | Login & Generate JWT |
| `/api/upload/orders` | POST | Upload Order CSV |
| `/api/upload/settlement` | POST | Upload Settlement CSV |

---

## Security

- JWT Authentication
- Stateless Session Management
- Role-based Access
- CORS Configuration

---

## Profit Calculation Logic

For each SKU:

```text
Revenue = Order Item Price
Cost = Quantity × Cost Price
Profit = Revenue − Cost − Amazon Fees
