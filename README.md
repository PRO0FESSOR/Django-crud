# Django-crud

# Django CRUD Project

This is a Django CRUD (Create, Read, Update, Delete) project that demonstrates a basic implementation of a web application for managing data using the Django framework. The project provides a simple interface for performing CRUD operations on a database.

## Requirements

To run this project, you need to have the following installed:

- Python (version 3.7 or higher)
- Django (version 3.2 or higher)
- SQLite or any other database backend supported by Django (optional)

## Installation

1. Clone or download this repository to your local machine.
2. Open a terminal or command prompt and navigate to the project's root directory.
3. Create a virtual environment to isolate the project's dependencies:

```bash
python -m venv env
```

4. Activate the virtual environment:

**Windows**
```bash
env\Scripts\activate
```

**Unix or Linux**
```bash
source env/bin/activate
```

5. Install the project's dependencies:

```bash
pip install -r requirements.txt
```

## Configuration

Before running the project, you need to configure the database settings. By default, the project uses SQLite as the database backend. However, you can modify the `settings.py` file to use a different database if desired.

1. Open the `settings.py` file located in the `crud_project` directory.
2. Find the `DATABASES` section and update the `default` configuration to match your database settings. For example, if you want to use SQLite, the default configuration looks like this:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    }
}
```

3. Save the changes and close the file.

## Running the Project

To run the project, follow these steps:

1. Make sure the virtual environment is activated.
2. Navigate to the project's root directory.
3. Run the following command to apply the database migrations:

```bash
python manage.py migrate
```

4. Start the development server:

```bash
python manage.py runserver
```

5. Open a web browser and visit `http://localhost:8000` to access the application.

## Usage

The application provides a simple interface for managing data. You can perform the following operations:

- **Create**: Click on the "Add Item" button to create a new item. Fill in the required fields and click "Save" to add the item to the database.
- **Read**: The main page displays a list of all items in the database. Each item shows its details, and you can click on an item to view its individual page.
- **Update**: On the item's individual page, click the "Edit" button to modify the item's information. Update the fields as needed and click "Save" to apply the changes.
- **Delete**: On the item's individual page, click the "Delete" button to remove the item from the database.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify it according to your needs.

## Contributing

If you have any suggestions, improvements, or issues, please submit them to the [GitHub repository](https://github.com/your/repository). Contributions are welcome!

## Acknowledgments

This project was inspired by the need for a simple Django CRUD application. Special thanks to the Django community for their excellent documentation and resources.

If you have any questions or need further assistance , feel free to contact me at [siddharth96549@example.com](mailto:your-email@example.com). Thank you for using this project! 