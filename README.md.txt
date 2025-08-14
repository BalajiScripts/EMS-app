# EMS App (Spring Boot + React/Vite)

## 📂 Structure
- **ems-backend** → Spring Boot REST API (port 8080)
- **ems-frontend** → React (Vite) UI

## ⚙️ Requirements
- JDK 17+
- Node.js 18+ & npm
- MySQL (or your DB)

## 🚀 Setup (any laptop)
1. **Backend**
   - Create DB `ems` (or update URL in `application.properties`)
   - Copy `src/main/resources/application-example.properties` → `application.properties` and set DB credentials
   - Run:
     ```bash
     ./mvnw spring-boot:run
     ```
     *(or run `EmsBackendApplication` in IntelliJ)*

2. **Frontend**
   - Go to `ems-frontend`
   - Copy `.env.example` → `.env`
   - Install packages:
     ```bash
     npm install
     ```
   - Start dev server:
     ```bash
     npm run dev
     ```

## 🔗 API URL
React app uses `VITE_API_BASE_URL` from `.env`:
```env
VITE_API_BASE_URL=http://localhost:8080
