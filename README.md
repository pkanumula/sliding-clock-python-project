# Sliding Clock - A Flask & JavaScript Project

A full-stack web application that displays a real-time clock with a smooth sliding animation for the digits.

## Table of Contents

- [Project Description](#project-description)
- [Live Demo](#live-demo)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Application Flow](#application-flow)
- [File Structure](#file-structure)

## Project Description

The **Sliding Clock** is a minimalist web application designed to showcase a fluid user interface powered by a Python backend. The Flask web framework serves as the backbone, providing the current time through a RESTful API endpoint. The frontend utilizes vanilla JavaScript to consume this API and dynamically render the time, creating an elegant "sliding" visual effect for each digit change.

## Live Demo

**(Highly recommended to create a short GIF of the clock in action!)**

![Demo GIF](https://i.imgur.com/YOUR_IMAGE_URL.gif)

## Features

- ✅ Real-time, second-by-second updates.
- ✅ Smooth CSS-based animations for digit transitions.
- ✅ Clean, responsive, and centered layout.
- ✅ Efficient client-server communication.
- ✅ Well-documented and cleanly structured code.

## Technologies Used

-   **Backend**:
    -   ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
    -   ![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
-   **Frontend**:
    -   ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
    -   ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
    -   ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

## Setup and Installation

To run this project locally, please follow these steps:

1.  **Clone the repository to your local machine:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/sliding-clock-python-project.git](https://github.com/YOUR_USERNAME/sliding-clock-python-project.git)
    ```

2.  **Navigate into the project directory:**
    ```bash
    cd sliding-clock-python-project
    ```

3.  **Install the necessary Python package(s):**
    ```bash
    pip install -r requirements.txt  
    # (Note: For this, first create a requirements.txt file with 'Flask' inside it)
    # Or simply:
    pip install Flask
    ```

4.  **Execute the main application script:**
    ```bash
    python app.py
    ```
    The server will start on `http://127.0.0.1:5000`.

## Application Flow

1.  The user navigates to the root URL (`/`).
2.  Flask renders the `index.html` template.
3.  The browser loads the linked `script.js` file.
4.  The `script.js` sets an interval to send a `GET` request to the `/time` endpoint every 1000ms.
5.  The Flask `/time` route calculates the current time and returns it as JSON.
6.  The JavaScript receives the JSON and updates the inner HTML of the clock digits.
7.  CSS transitions handle the visual "sliding" animation when the content of the digits changes.

## File Structure
