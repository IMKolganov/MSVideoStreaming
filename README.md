# MSVideoStreaming
# Live Video Stream Application

This application provides a live video stream using a webcam and serves it through a Flask web server. It also supports WebSocket connections using Flask-SocketIO.

## Features

- Streams live video from the webcam.
- Serves static files such as HTML using Flask.
- Supports WebSocket connections for real-time communication.

## Technologies Used

- **Flask**: A lightweight WSGI web application framework in Python.
- **Flask-SocketIO**: Adds WebSocket support to Flask applications.
- **OpenCV**: Library used for computer vision tasks, including capturing video.
- **Flask-CORS**: Handles Cross-Origin Resource Sharing (CORS) for Flask.

## Prerequisites

- Python 3.10 or later
- pip (Python package installer)

## Installation

1. **Clone the Repository**

    ```sh
    git clone https://github.com/yourusername/your-repo.git
    cd your-repo
    ```

2. **Create and Activate a Virtual Environment**

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies**

    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. **Run the Flask Application**

    ```sh
    python app.py
    ```

2. **Access the Application**

    - Open a web browser and navigate to `http://localhost:5003/` to view the live video stream.
    - The video feed is available at `http://localhost:5003/video_feed`.

3. **WebSocket Connections**

    - The application supports WebSocket connections, which you can use to send and receive real-time messages.
    - Use appropriate WebSocket clients or libraries to interact with the server.

## Docker

To run the application using Docker, follow these steps:

1. **Build the Docker Image**

    ```sh
    docker build -t live-video-stream-app .
    ```

2. **Run the Docker Container**

    ```sh
    docker run -p 5003:5003 live-video-stream-app
    ```

3. **Access the Application**

    - Open a web browser and navigate to `http://localhost:5003/` to view the live video stream.

## Code Overview

- `app.py`: The main application file that sets up the Flask server, handles video streaming, and manages WebSocket connections.
- `requirements.txt`: Lists all Python dependencies needed to run the application.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or issues, please open an issue on the GitHub repository or contact the project maintainer.

