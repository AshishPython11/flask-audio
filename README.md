# Flask Audio API

This project is a backend server built using Flask that implements a REST API for processing audio based on its length. The API allows users to upload audio files and processes them according to specified conditions.

## Project Structure

```
flask-audio-api
├── app
│   ├── __init__.py
│   ├── routes.py
│   ├── services
│   │   └── audio_processor.py
│   └── models
│       └── __init__.py
├── tests
│   ├── __init__.py
│   └── test_routes.py
├── requirements.txt
├── config.py
└── README.md
```

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd flask-audio-api
   ```

2. Create a virtual environment:
   ```
   python -m venv venv
   ```

3. Activate the virtual environment:
   - On Windows:
     ```
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```
     source venv/bin/activate
     ```

4. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Usage

To run the Flask application, use the following command:
```
flask run
```

The API will be available at `http://127.0.0.1:5000`.

## API Endpoints

### Process Audio

- **Endpoint:** `/process-audio`
- **Method:** `POST`
- **Description:** Accepts an audio file and processes it based on its length. If the audio length exceeds 60 seconds, it trims the audio to its middle segment.

## Running Tests

To run the tests, use the following command:
```
pytest
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.