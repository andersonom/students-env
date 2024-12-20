# Students Environment

This repository contains the environment setup for the Students Manager application, including Docker configurations and Visual Studio solution files.

## Project Structure

- `StudentsManager/`: Contains the Students Manager backend services.
- `StudentsManager-UI/`: Contains the Students Manager frontend application.
- `.vscode/`: Contains Visual Studio Code configurations for debugging and tasks.
- `.dockerignore`: Specifies files and directories to be ignored by Docker.
- `.gitignore`: Specifies files and directories to be ignored by Git.
- `docker-compose.yml`: Defines the Docker services for the application.
- `docker-compose.override.yml`: Overrides Docker service configurations for development.
- `Students.Environment.sln`: Visual Studio solution file for the project.

## Prerequisites

- Docker
- Docker Compose
- .NET Core SDK
- Visual Studio or Visual Studio Code

## Getting Started

1. Clone the repository:
    ```sh
    git clone --recurse-submodules https://github.com/andersonom/students-env.git
    cd students-env
    ```

2. Build and run the Docker containers:
    ```sh
    docker-compose up --build
    ```

3. Open the solution in Visual Studio or Visual Studio Code:
    ```sh
    code Students.Environment.sln
    ```

## Services

- **studentsmanager.ui**: The frontend application running on port 8088.
- **studentsmanager.api**: The backend API running on port 8089.
- **redis.students**: Redis service running on port 16379.
- **db**: SQL Server database running on port 1401.

## Development

### Building the Project

To build the project, run the following command:
```sh
dotnet build StudentsManager-UI/StudentsManager.UI.csproj
```

### Running the Project

To run the project, use the following command:
```sh
dotnet run --project StudentsManager-UI/StudentsManager.UI.csproj
```

### Debugging

To debug the project in Visual Studio Code, use the provided launch configuration in `launch.json`.

### Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

### License

This project is licensed under the MIT License.

