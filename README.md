# GradMaster Project
Central repository for the development of the GradMaster project.

## Submodules
Here are links to the different parts of the project:

- [Core](https://github.com/jbarus/GradMasterCore)
- [Backend](https://github.com/jbarus/GradMasterBackend)
- [Desktop App](https://github.com/jbarus/GradMasterDesktop)

## Running the Containerized Part of the Program
Follow these steps to set up and run the containerized portion of the application:

1. Clone this repository and navigate to the folder:
   ```bash
   git clone https://github.com/jbarus/GradMaster.git
   cd GradMaster
   ```

2. Create a `.env` file and fill it with the required configuration. Refer to the provided `.env.template` file for guidance. Below is an explanation of the variables:
    - `RABBITMQ_HOST` - The host address (e.g., `192.168.1.2`, as specified in `docker-compose.yml`).
    - `RABBITMQ_PORT` - The port number (default is `5672`).
    - `RABBITMQ_USERNAME` - Username for RabbitMQ.
    - `RABBITMQ_PASSWORD` - Password for RabbitMQ.

3. Build the Docker images:
   ```bash
   docker-compose build --no-cache
   ```

4. Start the Docker containers:
   ```bash
   docker-compose up
   ```

## Running the Desktop Application
Currently, you need IntelliJ IDEA to run the desktop application. Follow these steps:

1. Open IntelliJ IDEA and clone the repository for the desktop application:
   ```
   git clone https://github.com/jbarus/GradMasterDesktop.git
   ```

2. In IntelliJ IDEA, right-click on `GradMasterDesktopApplication` and select **Run**.

---