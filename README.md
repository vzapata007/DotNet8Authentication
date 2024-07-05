# DotNet8Authentication

DotNet8Authentication is an ASP.NET Core project that implements user authentication and authorization using ASP.NET Core Identity. It also provides a simple API endpoint for fetching weather forecasts.

## Technologies Used

- ASP.NET Core
- Entity Framework Core
- ASP.NET Core Identity
- SQL Server
- Swagger for API documentation
- Swashbuckle for integrating Swagger with ASP.NET Core
- Front-end: React with Vite, ASP.NET MVC, or another technology (please update based on your specific implementation)

## Getting Started

Follow these instructions to set up and run the project locally.

### Prerequisites

- .NET SDK 6.0 or later
- SQL Server
- (Node.js and npm for front-end development, if applicable)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/DotNet8Authentication.git
    cd DotNet8Authentication
    ```

2. Set up the database:
    - Update the connection string in `appsettings.json` to match your SQL Server configuration.
    - Run the following commands to create and apply the database migrations:
      ```sh
      dotnet ef database update
      ```

3. Run the project:
    ```sh
    dotnet run
    ```

4. Open a browser and navigate to `https://localhost:5001/swagger` to view the Swagger UI and explore the API endpoints.


### API Endpoints

- `GET /WeatherForecast`: Fetches weather forecast data. This endpoint is protected by authorization and requires a valid JWT token in the Authorization header.

### Configuration

- `appsettings.json`: Contains configuration settings, including the database connection string and logging levels.

### Migrations

The initial migration creates the tables required for ASP.NET Core Identity:
- `AspNetUsers`
- `AspNetRoles`
- `AspNetUserRoles`
- `AspNetUserClaims`
- `AspNetUserLogins`
- `AspNetUserTokens`
- `AspNetRoleClaims`

### Authentication

This project uses ASP.NET Core Identity for authentication and authorization. Swagger is configured to accept a bearer token in the Authorization header.

### Front-end

- **React with Vite:** If the front-end is React with Vite, follow the instructions specific to setting up and running a React application.
- **ASP.NET MVC:** If the front-end is ASP.NET MVC, follow the instructions for setting up and running an ASP.NET MVC application.
- **Other Front-end Technologies:** Update this section based on the front-end technology you are using.

### Example Front-end Setup (React with Vite)

If using **React with Vite**, you might need to follow these steps:

1. Navigate to the front-end directory (if separate):
    ```sh
    cd front-end
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

3. Run the development server:
    ```sh
    npm run dev
    ```

4. Open a browser and navigate to `http://localhost:3000` to view the React application.

### Example Front-end Setup (ASP.NET MVC)

If using **ASP.NET MVC**, you might need to follow these steps:

1. Navigate to the MVC front-end directory (if separate):
    ```sh
    cd FrontEndMvc
    ```

2. Restore the dependencies:
    ```sh
    dotnet restore
    ```

3. Run the application:
    ```sh
    dotnet run
    ```

4. Open a browser and navigate to `http://localhost:5000` to view the ASP.NET MVC application.

---
