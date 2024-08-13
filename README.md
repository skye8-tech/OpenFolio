# OpenFolio

Welcome to **OpenFolio**! This collaborative project is aimed at creating a dynamic personal portfolio homepage with fully integrated backend features. Each section of the portfolio is managed by a different developer, ensuring a modular and efficient approach to building a robust portfolio system.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Overview

**OpenFolio** is designed to help developers showcase their skills, projects, and other professional details in an elegant and dynamic manner. The project is divided into sections, each handled by different backend developers, focusing on both frontend and backend aspects.

## Features

- **Skills Section:** Display your technical skills with dynamic progress bars.
- **Projects Section:** Showcase your projects with details like title, description, and technologies used.
- **Contact Form:** A fully functional contact form with validation and database integration.
- **Hero/About Me Section:** Introduce yourself with a dynamic welcome message and bio.

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** PHP
- **Database:** MySQL
- **Version Control:** Git/GitHub

## Setup and Installation

### Prerequisites

- **PHP:** Version 7.4 or higher
- **MySQL:** Version 5.7 or higher
- **Composer:** Latest version (for managing PHP dependencies)
- **Git:** Version control

### Installation Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/skye8-tech/OpenFolio.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd OpenFolio
   ```

3. **Install PHP dependencies:**

   ```bash
   composer install
   ```

4. **Set up the environment file:**

   Copy the `.env.example` file to `.env` and update the database credentials:

   ```bash
   cp .env.example .env
   ```

5. **Set up the database:**

   - Create a new database in MySQL.
   - Run any necessary SQL scripts to create tables and set up the schema. Check the `database/` folder or relevant documentation for these scripts.

6. **Serve the application:**

   ```bash
   php -S localhost:8000
   ```

7. **Open your browser:**

   Visit [http://localhost:8000](http://localhost:8000) to view the portfolio homepage.


8. **Project Structure**
    ```
        OpenFolio/
        │
        ├── assets/
        │   ├── css/
        │   │   └── style.css
        │   ├── js/
        │   │   └── script.js
        │   └── images/
        │       └── (your image files)
        │
        ├── config/
        │   └── config.php           # Database and application configuration
        │
        ├── public/
        │   ├── index.php            # Main entry point of the application
        │   └── .htaccess            # Configuration for URL rewriting and security
        │
        ├── src/
        │   ├── Controllers/
        │   │   ├── HomeController.php # Controller for handling homepage logic
        │   │   ├── SkillsController.php # Controller for skills section
        │   │   └── ProjectsController.php # Controller for projects section
        │   ├── Models/
        │   │   ├── Skill.php         # Model for handling skills data
        │   │   ├── Project.php       # Model for handling project data
        │   │   └── Contact.php       # Model for handling contact form data
        │   └── Views/
        │       ├── header.php        # Header part of HTML layout
        │       ├── footer.php        # Footer part of HTML layout
        │       ├── home.php          # View for homepage
        │       ├── skills.php        # View for skills section
        │       ├── projects.php      # View for projects section
        │       └── contact.php       # View for contact form
        │
        ├── database/
        │   └── migrations/           # SQL scripts or migration files for setting up the database schema
        │
        ├── logs/
        │   └── app.log               # Log files for debugging and tracking
        │
        ├── tests/
        │   └── (unit and integration tests, if applicable)
        │
        ├── .env                      # Environment variables (not included in version control)
        ├── composer.json             # Composer dependencies and configurations (if using Composer)
        ├── composer.lock             # Composer lock file (if using Composer)
        └── README.md                 # Project documentation
    ```

## Usage

Each developer will work on their assigned section, implementing both frontend and backend features. Please ensure you push changes to your respective branches and submit pull requests for merging into the main branch.

## Contributing

1. **Fork the repository.**
2. **Create your branch:** `git checkout -b feature/YourFeature`
3. **Commit your changes:** `git commit -m 'Add some feature'`
4. **Push to the branch:** `git push origin feature/YourFeature`
5. **Open a pull request.**

Please make sure to update tests as appropriate and follow the code style guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Special thanks to all contributors who have made this project possible. Each section of this portfolio has been carefully crafted to ensure a cohesive and dynamic user experience.
