# Joke Web App

Welcome to the Jokes Management System! This ASP.NET project allows you to manage a collection of jokes with functionalities to add, update, delete, and search jokes. The project uses a MySQL database to store the jokes.

## Features

- Add a new joke
- Update an existing joke
- Delete a joke
- List all jokes
- Search for jokes using keywords

## Screenshots

Here are some screenshots of the application:

### Home Page
![Home Page](screenshots/home.png)

### Add Joke
![Add Joke](screenshots/add-joke.png)

### List Jokes
![List Jokes](screenshots/list-jokes.png)

### Search Jokes
![Search Jokes](screenshots/search-jokes.png)
## Getting Started

### Prerequisites

Before you begin, ensure you have the following:

- [.NET SDK](https://dotnet.microsoft.com/download)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/)
- [Visual Studio](https://visualstudio.microsoft.com/) or any other preferred IDE

### Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/yourusername/jokes-management-system.git
    cd jokes-management-system
    ```

2. **Setup MySQL Database:**

    - Create a database named `jokesdb`.
    - Run the following SQL script to create the `jokes` table:

        ```sql
        CREATE DATABASE jokesdb;
        USE jokesdb;

        CREATE TABLE jokes (
            id INT AUTO_INCREMENT PRIMARY KEY,
            question VARCHAR(255) NOT NULL,
            answer TEXT NOT NULL
        );
        ```

3. **Update Database Connection String:**

    In the `appsettings.json` file, update the connection string to match your MySQL server configuration:

    ```json
    "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Database=jokesdb;User=root;Password=yourpassword;"
    }
    ```

4. **Build and Run the Project:**

    Open the project in Visual Studio and run it, or use the .NET CLI:

    ```sh
    dotnet build
    dotnet run
    ```

## Usage

Once the application is running, you can access it at `http://localhost:5000` (or the port specified in your launch settings).

### Adding a Joke

- Navigate to the "Add Joke" section.
- Enter the joke question and answer.
- Click "Submit" to save the joke.

### Updating a Joke

- Navigate to the "List Jokes" section.
- Click "Edit" next to the joke you want to update.
- Modify the joke question and answer.
- Click "Update" to save the changes.

### Deleting a Joke

- Navigate to the "List Jokes" section.
- Click "Delete" next to the joke you want to remove.
- Confirm the deletion.

### Searching for a Joke

- Navigate to the "Search Jokes" section.
- Enter a keyword related to the joke you are looking for.
- Click "Search" to find relevant jokes.


## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any improvements or bug fixes.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

Your Name - [@yourtwitterhandle](https://twitter.com/yourtwitterhandle) - yourname@example.com

Project Link: [https://github.com/yourusername/jokes-management-system](https://github.com/yourusername/jokes-management-system)

---

Happy coding! 😊
