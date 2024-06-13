# My Flask App

This is a simple Flask web application.

## Prerequisites

Before you begin, ensure you have met the following requirements:
- You have installed Python 3.6 or later.
- You have installed Git.

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/DonPedro428/my_flask_app.git
    cd my_flask_app
    ```

2. **Create a Virtual Environment**:
    - On Windows:
        ```bash
        python -m venv venv
        venv\Scripts\activate
        ```
    - On macOS/Linux:
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Running the Application

1. **Ensure the Virtual Environment is Activated**:
    - On Windows:
        ```bash
        venv\Scripts\activate
        ```
    - On macOS/Linux:
        ```bash
        source venv/bin/activate
        ```

2. **Run the Application**:
    ```bash
    python run.py
    ```

3. **Access the Application**:
    - Open your web browser and navigate to `http://127.0.0.1:5000` (or the specified port if different).

## Debugging and Development

- The application runs with debug mode enabled by default. This means that it will automatically reload for code changes and show an interactive debugger in the browser for uncaught exceptions.

## Deployment

For deploying to a production environment, consider using a production WSGI server like Gunicorn or uWSGI. Below are basic instructions for deploying with Gunicorn.

1. **Install Gunicorn**:
    ```bash
    pip install gunicorn
    ```

2. **Run the Application with Gunicorn**:
    ```bash
    gunicorn -w 4 -b 0.0.0.0:8000 run:app
    ```
    - This runs the app with 4 worker processes on port 8000. Adjust the number of workers and port as necessary for your deployment.

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-foo`).
3. Make your changes and commit them (`git commit -m 'Add some foo'`).
4. Push to the branch (`git push origin feature-foo`).
5. Create a Pull Request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
