# Security Camera with Python

A Python-based security camera application using OpenCV to detect motion or faces and record footage automatically. The system starts recording upon detection and stops after a specified duration of no activity.

---

## Features

- **Motion Detection**: Detects faces and bodies using pre-trained Haar cascades.
- **Automatic Recording**: Starts recording when motion is detected and stops after a period of inactivity.
- **Customizable Settings**: Easily adjust detection and recording parameters.
- **Real-Time Monitoring**: Displays the camera feed with detection feedback.

---

## Project Structure

- **`tutorial.py`**: Main script implementing the security camera functionality.

---

## Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. Install dependencies:
   ```bash
   pip install opencv-python
   ```

3. Run the script:
   ```bash
   python tutorial.py
   ```

---

## How It Works

1. **Initialization**:
   - The script initializes the camera feed using OpenCV.
   - Haar cascade classifiers are loaded for face and body detection.

2. **Detection and Recording**:
   - If a face or body is detected, recording begins immediately.
   - Recording stops after 5 seconds of no motion detection (configurable).

3. **Output**:
   - Recorded videos are saved in the current directory with timestamps as filenames.
   - The live feed is displayed with real-time detection.

---

## Configuration

- **Recording Duration**:
  Modify `SECONDS_TO_RECORD_AFTER_DETECTION` in `tutorial.py` to change the recording time after detection.

- **Detection Sensitivity**:
  Adjust parameters in `detectMultiScale()` (e.g., scale factor and minimum neighbors) for fine-tuning face and body detection.

---

## Dependencies

The project requires the following Python libraries:

- `opencv-python`

Install it using:
```bash
pip install opencv-python
```

---

## Usage

### Running the Security Camera
Execute the main script to start monitoring:
```bash
python tutorial.py
```

### Stopping the Camera
Press `q` in the live feed window to stop the camera and exit the program.

---

## Contributing

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add new feature'
   ```
4. Push the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request.

---

## License

This project is licensed under the MIT License. See `LICENSE` for more details.

---

## Acknowledgments

- **OpenCV**: For providing tools for image and video processing.
- **Haar Cascades**: For pre-trained models used in motion detection.

---
