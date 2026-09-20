# HRMS SaaS Product

A comprehensive Human Resource Management System (HRMS) built as a multi-tenant SaaS platform. This application streamlines HR operations including employee management, attendance tracking, payroll processing, and internal ticketing.

## 🚀 Tech Stack

### Frontend (`/hrms-frontend`)
* **Framework:** React
* **Build Tool:** Vite
* **Language:** TypeScript
* **Styling/UI:** CSS / (Add your UI library here, e.g., TailwindCSS, MUI)

### Backend (`/HrmsBackend`)
* **Framework:** .NET 10 (ASP.NET Core Web API)
* **Language:** C#
* **Architecture:** Modular Monolith / Clean Architecture
* **Modules Included:**
  * `Identity`: Authentication, authorization, and user management.
  * `Organization`: Company structure, departments, and employee profiles.
  * `Attendance`: Time tracking, leave management, and shift scheduling.
  * `Payroll`: Salary calculations, deductions, and payslip generation.
  * `Ticketing`: Internal HR helpdesk and request tracking.

## 📁 Project Structure

```text
HRMS-SaaS-Product/
├── hrms-frontend/            # React/Vite frontend application
│   ├── public/               # Static assets
│   ├── src/                  # React components, pages, and hooks
│   └── package.json          # Frontend dependencies
│
└── HrmsBackend/              # .NET Backend solution
    ├── src/
    │   ├── Api/              # Main API entry point (Controllers & Program.cs)
    │   ├── Modules/          # Domain-specific modules (Attendance, Identity, etc.)
    │   └── Shared/           # Cross-cutting concerns, shared contracts, and infrastructure
    └── HrmsBackend.sln       # Visual Studio Solution file
```

## 🛠️ Getting Started

### Prerequisites
* [Node.js](https://nodejs.org/) (v18 or higher recommended)
* [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)
* A Code Editor (VS Code, Visual Studio, or JetBrains Rider)

### Running the Frontend

1. Navigate to the frontend directory:
   ```bash
   cd hrms-frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
4. Open your browser and navigate to the local URL provided by Vite (usually `http://localhost:5173`).

### Running the Backend

1. Navigate to the backend API directory:
   ```bash
   cd HrmsBackend/src/Api
   ```
2. Restore dependencies and run the application:
   ```bash
   dotnet restore
   dotnet run
   ```
3. The API will start and should be accessible via `http://localhost:5000` or `https://localhost:5001`. You can typically view the Swagger documentation at `/swagger`.

## 🤝 Contributing

1. Create a new branch for your feature (`git checkout -b feature/AmazingFeature`)
2. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
3. Push to the branch (`git push origin feature/AmazingFeature`)
4. Open a Pull Request

## 📄 License

This project is proprietary and confidential.
