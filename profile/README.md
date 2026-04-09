#  Travel Planner - Full Stack Application

<p align="center">
  <img src="https://img.shields.io/badge/Java_21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" />
  <img src="https://img.shields.io/badge/Angular_17-DD0031?style=for-the-badge&logo=angular&logoColor=white" />
  <img src="https://img.shields.io/badge/Oracle_DB-F80000?style=for-the-badge&logo=oracle&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white" />
</p>

##  Overview
**Travel Planner** is a high-performance, full-stack platform designed for global travel management. It features a robust **Spring Boot 3** backend with **Oracle Database** and a modern **Angular ** frontend. The system provides seamless user experiences from secure authentication to complex data imports and administrative management.

---

##  Core Features

###  User Capabilities
* **Secure Authentication:** Multi-step registration and JWT-based secure login.
* **Personalized Wishlist:** Users can save, view, and manage their favorite destinations instantly.
* **Optimistic UI Updates:** Real-time feedback when liking/saving destinations.

###  Administrative (Admin Panel)
* **User Management:** Full control over user roles, account status (Active/Inactive), and details.
* **Destination Catalog:** CRUD operations to manage global travel spots with rich metadata.
* **External Data Bulk Upload:** Integration with external APIs to fetch and import hundreds of destinations in seconds.
* **Role-Based Access Control (RBAC):** Strict security layers for Admin vs. User permissions.

---

##  Tech Stack

### **Backend (The Engine)**
* **Framework:** Spring Boot 3.x
* **Language:** Java 21
* **Database:** Oracle Database (Relational persistence)
* **Security:** Spring Security + JWT Tokens
* **Documentation:** Swagger / OpenAPI UI
* **Architecture:** Clean Architecture with DTOs and Service Layer

### **Frontend (The Experience)**
* **Framework:** Angular 17+ (Standalone Components)
* **State Management:** Angular Signals (Modern Reactivity)
* **Styling:** SCSS with custom Grid/Flexbox layouts
* **Responsiveness:** Fully mobile-friendly admin panel

---

##  API Documentation

###  Authentication (`auth-controller`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/auth/register` | Create a new user account |
| `POST` | `/auth/login` | Authenticate and receive a JWT token |

###  Destinations (`destination-controller`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/destinations` | Retrieve a list of all destinations |
| `POST` | `/destinations` | Add a new destination to the catalog |
| `GET` | `/destinations/{id}` | Get detailed info for a specific destination |
| `PATCH` | `/destinations/{id}` | Partially update destination details |
| `DELETE` | `/destinations/{id}` | Remove a destination from the system |

###  User Management (`user-controller`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/users` | List all registered users (Admin only) |
| `GET` | `/users/{userId}` | Get profile data for a specific user |
| `PUT` | `/users/{userId}` | Update user profile information |
| `PATCH` | `/users/{userId}` | Modify specific user fields |
| `DELETE` | `/users/{userId}` | Delete a user account |
| `GET` | `/users/role` | Check/Verify user authorization roles |

###  Favorites (`favorite-destination-controller`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/favorites` | Fetch the current user's list of favorites |
| `POST` | `/favorites/{id}` | Add a specific destination to favorites |
| `DELETE` | `/favorites/{id}` | Remove a destination from favorites |

###  External Data (`external-destination-controller`)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/externalDestinations` | Fetch available data from external sources |
| `POST` | `/externalDestinations/name` | Search external destinations by name |
| `POST` | `/externalDestinations/import` | Import selected external data into local database |

---

## Getting Started

### Backend Setup
1. Clone the repo: `git clone https://github.com/TravelPlanner-Organization/TravelDestination.git`
2. Update `application.properties` with your Oracle DB credentials.
3. Build and run: `mvn spring-boot:run`

### Frontend Setup
1. Clone the repo: `git clone https://github.com/TravelPlanner-Organization/TravelDestinationFrontEnd.git`
2. Install dependencies: `npm install`
3. Launch development server: `ng serve`

---

## Project Showcase

###  User Interface (Frontend)
## Auth
<img width="1854" height="911" alt="image" src="https://github.com/user-attachments/assets/77a97ecc-17d5-40b9-b2e0-46c43dc2678d" />
<img width="1849" height="910" alt="image" src="https://github.com/user-attachments/assets/b084a291-0d50-40d5-b248-ac28fcc5d91d" />

## User Dashboard
<img width="1860" height="912" alt="image" src="https://github.com/user-attachments/assets/c04abb07-41d7-402b-b5e1-f8fdaab9b4d8" />
<img width="1841" height="906" alt="image" src="https://github.com/user-attachments/assets/414403e1-456b-4ede-81eb-e1e5345f89aa" />

## Admin Dashboard
<img width="1860" height="908" alt="image" src="https://github.com/user-attachments/assets/9247caa1-ccfa-4b40-a9f3-64d21b352337" />
<img width="1455" height="908" alt="image" src="https://github.com/user-attachments/assets/17694daa-9006-42dc-b05a-dcd697933ed0" />
<img width="1531" height="911" alt="image" src="https://github.com/user-attachments/assets/57b2ecf8-5280-4209-b0e2-47441656f0fc" />
<img width="1455" height="908" alt="image" src="https://github.com/user-attachments/assets/6d1909b0-c4fa-4016-9561-02fd823cf2e0" />
<img width="1843" height="714" alt="image" src="https://github.com/user-attachments/assets/380ef647-14f8-493e-b2fa-7363d919d54c" />

###  Backend & API Integration
<img width="1600" height="842" alt="image" src="https://github.com/user-attachments/assets/422cc880-1555-4e02-ab36-5fd79537b323" />
<img width="1571" height="490" alt="image" src="https://github.com/user-attachments/assets/263f045a-2dc3-4294-b634-8f23e8fbf642" />
