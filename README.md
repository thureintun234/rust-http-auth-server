# Rust Auth with Audit

A simple authentication API built with Rust, featuring JWT-based authentication and audit logging. Uses PostgreSQL as the database.

## Features

- User registration and login
- JWT authentication
- Audit logging for key actions
- Environment-based configuration

## Used Technologies

- [actix-web](https://crates.io/crates/actix-web) – Web framework
- [actix-cors](https://crates.io/crates/actix-cors) – CORS support
- [sqlx](https://crates.io/crates/sqlx) – Async PostgreSQL ORM
- [argon2](https://crates.io/crates/argon2) – Password hashing
- [jsonwebtoken](https://crates.io/crates/jsonwebtoken) – JWT handling
- [dotenv](https://crates.io/crates/dotenv) – Environment variable management
- [serde](https://crates.io/crates/serde) & [serde_json](https://crates.io/crates/serde_json) – Serialization
- [chrono](https://crates.io/crates/chrono) – Date and time
- [uuid](https://crates.io/crates/uuid) – UUID generation
- [validator](https://crates.io/crates/validator) – Input validation
- [utoipa](https://crates.io/crates/utoipa), [utoipa-swagger-ui](https://crates.io/crates/utoipa-swagger-ui), [utoipa-redoc](https://crates.io/crates/utoipa-redoc), [utoipa-rapidoc](https://crates.io/crates/utoipa-rapidoc) – OpenAPI documentation

## Getting Started

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install)
- [PostgreSQL](https://www.postgresql.org/download/)

### Setup

1. **Clone the repository:**

   ```sh
   git clone <your-repo-url>
   cd rust-http-auth-server
   ```

2. **Configure environment variables:**

   Create a `.env` file in the project root:

   ```
   DATABASE_URL=postgres://postgres:password@localhost:5432/mydatabase
   JWT_SECRET_KEY=your_jwt_secret_key_here
   JWT_MAXAGE=3600
   PORT=8000
   ```

3. **Run database migrations** (if applicable).

4. **Run the server:**
   ```sh
   cargo run
   ```

## Usage

- The API will be available at `http://localhost:8000`.
- Use tools like Postman or curl to interact with the
