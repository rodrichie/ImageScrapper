# Image Scrapper

A simple Flask web application that allows users to search for images by entering a keyword and retrieving relevant images based on the search term.

## Features

- **Image Search**: Enter a keyword to search for relevant images.
- **Image Display**: Displays the retrieved images on the results page.

## How it Works

1. When the application starts, the user is presented with the `index.html` page.
2. The user enters a search keyword in the search box and presses the "Submit" button.
3. The application processes the request, searches for images, and shows the results on the `showImage.html` page.

## Installation

To get started with the Image Scrapper app, follow the steps below:

### 1. Clone the Repository

```bash
git clone https://github.com/rodrichie/ImageScrapper.git
```

### 2. Navigate to the Project Directory

```bash
cd ImageScrapper
```

### 3. Set Up the Virtual Environment

It's recommended to use a virtual environment to manage dependencies.

#### For Unix/macOS:
```bash
python3 -m venv venv
source venv/bin/activate
```

#### For Windows:
```bash
python -m venv venv
venv\Scripts\activate
```

### 4. Install Dependencies

Install Flask and other required dependencies using the [`requirements.txt`]
```bash
pip install -r requirements.txt
```

### 5. Set Up Environment Variables

Flask requires environment variables for the app to run correctly.

#### For Unix/macOS:
```bash
export FLASK_APP=app.py
export FLASK_ENV=development
```

#### For Windows:
```bash
set FLASK_APP=app.py
set FLASK_ENV=development
```

### 6. Ensure MongoDB is Running

Make sure MongoDB is installed and running on your machine before starting the application. You can start MongoDB with the following command (depending on your OS setup):

```bash
# Example for Unix/macOS
sudo service mongod start

# Example for Windows (if using MongoDB via a service)
net start MongoDB
```

### 7. Run the Flask Application

```bash
flask run
```

The application should now be running on `http://127.0.0.1:5000/` or `http://localhost:5000/`.

## Usage

1. Navigate to `http://localhost:5000/` in your web browser.
2. Enter a keyword in the search box on the home page (`index.html`).
3. Click the "Submit" button to start the search.
4. The application will display the results on the `showImage.html` page, showing relevant images based on the search keyword.

## License

This project is licensed under the [MIT License](LICENSE).
