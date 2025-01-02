

# Task Management System

This is a Task Management System project built with Spring Boot for the backend and Next.js for the frontend. The project allows users to manage tasks, organizations, and users with different roles and permissions.

## Project Structure

```
.
├── backend
│   ├── mvnw
│   ├── 

mvnw.cmd


│   ├── 

pom.xml


│   └── src
│       ├── main
│       │   ├── java
│       │   │   └── com
│       │   │       └── taskify
│       │   │           └── app
│       │   │               ├── config
│       │   │               ├── controller
│       │   │               ├── dto
│       │   │               ├── model
│       │   │               ├── repository
│       │   │               └── service
│       │   └── resources
│       │       └── 

application.properties


│       └── test
│           └── java
│               └── com
│                   └── phegondev
│                       └── usersmanagementsystem
├── frontend
│   ├── .gitignore
│   ├── .next
│   ├── app
│   ├── components
│   ├── context
│   ├── hooks
│   ├── public
│   ├── styles
│   ├── 

package.json


│   ├── 

postcss.config.mjs


│   ├── 

tailwind.config.ts


│   ├── 

tsconfig.json


│   └── 

README.md


└── .gitignore
```

## Backend

The backend is built with Spring Boot and provides RESTful APIs for managing tasks, users, and organizations. It uses JWT for authentication and authorization.

### Prerequisites

- Java 21
- Maven
- MySQL

### Setup

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd backend
   ```

2. Configure the database in 

application.properties

:
   ```properties


   spring.datasource.url=jdbc:mysql://localhost:3306/task_management_system


   spring.datasource.username=<your-username>
   spring.datasource.password=<your-password>
   ```

3. Run the application:
   ```sh
   ./mvnw spring-boot:run
   ```

## Frontend

The frontend is built with Next.js and provides a user interface for managing tasks, users, and organizations. It uses Tailwind CSS for styling.

### Prerequisites

- Node.js
- npm or yarn

### Setup

1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```

2. Install dependencies:
   ```sh
   npm install
   # or
   yarn install
   ```

3. Run the development server:
   ```sh
   npm run dev
   # or
   yarn dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Features

- User authentication and authorization with JWT
- Role-based access control (Admin, User)
- Manage tasks with different statuses (To Do, In Progress, Completed, Blocked)
- Manage users and organizations
- Kanban board for task management

## License

This project is licensed under the Apache License 2.0. See the LICENSE file for details.
