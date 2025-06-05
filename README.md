# Docker Stacks

A collection of Docker Compose stacks for various environments, categories, and services. This repository is designed to help you quickly set up and manage containerized services for development, testing, or home lab use.

---

## Repository Structure

- **Environment Level**  
  Top-level directories represent different environments (e.g., `Laptop`, `Home-Server`).  
  _Example: `Docker-Stacks/Laptop/`_

- **Category Level**  
  Within each environment, services are grouped by category (e.g., `Databases`, `DevOps`, `Monitoring`).  
  _Example: `Docker-Stacks/Laptop/Databases/`_

- **Service Level**  
  Each category contains directories for individual services (e.g., `mysql`, `oracle`, `mongodb`).  
  _Example: `Docker-Stacks/Laptop/Databases/oracle/`_

- **Service Version Level**  
  Each service may have one or more version-specific directories (e.g., `latest`, `v1`, `xe-11g`).  
  _Example: `Docker-Stacks/Laptop/Databases/oracle/latest/`_

---

## Getting Started

1. **Clone the Repository**
   ```sh
   git clone https://github.com/Jenil-Desai/Docker-Stacks.git
   cd Docker-Stacks
   ```

2. **Navigate to Your Desired Stack**
   - Choose your environment, category, service, and version.
   - Example:
     ```
     cd Laptop/Databases/oracle/latest
     ```

3. **Read the README.md at Each Level**
   - Each directory contains a `README.md` with specific setup and usage instructions.

4. **Configure Environment Variables**
   - Most stacks provide a `.env.example` file. Copy it to `.env` and adjust as needed.
     ```sh
     cp .env.example .env
     ```

5. **Start the Stack**
   - Use Docker Compose to start the services.
     ```sh
     docker compose up -d
     ```

---

## Contributing

1. Fork the repository.
2. Create a new branch for your changes.
3. Add or update stacks, documentation, or configurations.
4. Submit a pull request with a clear description.

---

## License

MIT License

---

## Contact

For questions, suggestions, or support, please contact:  
**Jenil Desai**  
[jenildev91@gmail.com](mailto:jenildev91@gmail.com)

---