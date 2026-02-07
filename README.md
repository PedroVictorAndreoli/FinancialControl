# FinancialControl

FinancialControl is a full‑stack personal finance control application with a Java/Spring Boot backend and a React/Vite frontend. It provides authentication, account management, transactions (movimentações), and dashboard views.

## Project Structure

- Back/: Spring Boot API (Java)
- client/: React + TypeScript web app (Vite)

## Features

- User authentication and security
- Account (Conta) management
- Transactions (Movimentações) management
- Dashboard summary views
- Input validation and localized messages

## Tech Stack

**Backend**
- Java
- Spring Boot
- Maven
- JPA/Hibernate
- Validation

**Frontend**
- React
- TypeScript
- Vite
- Axios

## Getting Started

### Backend (Back)

1. Ensure Java and Maven are installed.
2. Configure database settings in Back/src/main/resources/application.yml.
3. The backend reads initial data from Back/src/main/resources/import.sql (if enabled).
4. Run the Spring Boot application.

### Build and Run (bash)

#### Backend (Back)

- Build:

```bash
cd Back
mvn clean package
```

- Run (Maven):

```bash
cd Back
mvn spring-boot:run
```

- Run (JAR):

```bash
cd Back
java -jar target/*.jar
```

### Frontend (client)

1. Ensure Node.js is installed.
2. Install dependencies from client/package.json.
3. Configure API base URL in the frontend (see client/src/lib/axios.ts).
4. Start the Vite dev server.

#### Frontend (client)

- Build:

```bash
cd client
npm install
npm run build
```

- Run (dev):

```bash
cd client
npm install
npm run dev
```

## Configuration

- Backend configuration: Back/src/main/resources/application.yml
- Validation messages: Back/src/main/resources/ValidationMessages*.properties
- Frontend API client: client/src/lib/axios.ts

## Tests

- Backend tests are under Back/src/test/java.

## License

Specify the license for this project here.
