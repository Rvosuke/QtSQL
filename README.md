# SQL2Desktop Application

SQL2 is a user-friendly desktop application built with Qt Framework and SQL databases. The application allows users to perform basic SQL operations such as creating tables, inserting data, updating data, deleting data, and querying data.

## Structure of the project

The project is structured into various key components:

1. `main.cpp`: The entry point of the application. It creates a `QApplication` instance, loads appropriate language translations if available, and establishes connections between various window instances through the Qt signals and slots system.

2. `database.h` and `database.cpp`: These files define and implement the `Database` class, which manages the connection to the database and executes basic database operations.

3. `mainwindow.h` and `mainwindow.cpp`: These files define and implement the `MainWindow` class, which is a login window. The user enters database credentials here and logs in. Upon successful login, the `HomeWindow` is displayed.

4. `homewindow.h` (implementation not reviewed yet): This file defines the `HomeWindow` class, which is the main window of the application. The user can perform various database operations from this window. When a user clicks on the buttons for these operations, signals are emitted to open corresponding windows for each operation.

## How to use the application

1. Start the application, you will be greeted with the `MainWindow` (login window).
2. Enter the host, port, username, password, and database name in the respective fields and click on the login button.
3. If the login is successful, you will be redirected to the `HomeWindow` (main window) where you can perform various database operations.
4. Click on the buttons for various operations like creating tables, inserting data, updating data, deleting data, and querying data to perform the respective operation.

## Development

The project is built using the Qt Framework and requires Qt Creator for development. You also need to have a SQL database system installed and set up for the application to connect to. The application currently uses the QODBC driver to connect to the database.

## Contributing

Contributions are welcome. Please open an issue to discuss your ideas or submit a Pull Request with your changes.

## License

The project is licensed under [INSERT LICENSE HERE]. Please check the `LICENSE` file for more details.
