
# FFmpeg Video Converter

This is a simple FFmpeg-based video converter built using Python. The converter allows you to convert videos from one format to another, leveraging the powerful capabilities of FFmpeg.

## Features

- Convert videos between various formats (e.g., MP4, AVI, MKV, MOV, etc.)
- Customize conversion settings (bitrate, resolution, frame rate, etc.)
- Batch processing of multiple videos
- Simple and easy-to-use command-line interface

## Requirements

- Python 3.x
- FFmpeg

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/ffmpeg-video-converter.git
    cd ffmpeg-video-converter
    ```

2. **Install the required Python packages:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Ensure FFmpeg is installed and accessible from the command line:**
    - For Windows: [Download FFmpeg](https://ffmpeg.org/download.html), extract the files, and add the bin folder to your PATH environment variable.
    - For macOS: Install using Homebrew:
        ```bash
        brew install ffmpeg
        ```
    - For Linux: Install using your package manager, e.g., for Debian-based systems:
        ```bash
        sudo apt update
        sudo apt install ffmpeg
        ```

## Usage

### Command Line Interface

To convert a single video file, use the following command:

```bash
python convert.py --input input_video.mp4 --output output_video.avi --format avi --bitrate 1000k --resolution 1280x720 --framerate 30
```

**Options:**

- `--input`: Path to the input video file.
- `--output`: Path to the output video file.
- `--format`: Desired output video format (e.g., mp4, avi, mkv).
- `--bitrate`: Set the bitrate of the output video (e.g., 1000k for 1000 kbps).
- `--resolution`: Set the resolution of the output video (e.g., 1280x720).
- `--framerate`: Set the frame rate of the output video (e.g., 30 for 30 fps).

### Batch Processing

To convert all videos in a directory, use the following command:

```bash
python convert.py --input_dir /path/to/input/videos --output_dir /path/to/output/videos --format avi --bitrate 1000k --resolution 1280x720 --framerate 30
```

**Options:**

- `--input_dir`: Path to the directory containing input video files.
- `--output_dir`: Path to the directory to save the converted video files.
- `--format`: Desired output video format (e.g., mp4, avi, mkv).
- `--bitrate`: Set the bitrate of the output video (e.g., 1000k for 1000 kbps).
- `--resolution`: Set the resolution of the output video (e.g., 1280x720).
- `--framerate`: Set the frame rate of the output video (e.g., 30 for 30 fps).

## Example

Convert a single video from MP4 to AVI format:

```bash
python convert.py --input sample.mp4 --output sample.avi --format avi --bitrate 1000k --resolution 1280x720 --framerate 30
```

Batch convert all videos in a directory to MKV format:

```bash
python convert.py --input_dir ./videos --output_dir ./converted_videos --format mkv --bitrate 800k --resolution 640x480 --framerate 25
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgements

- [FFmpeg](https://ffmpeg.org) - The tool used for video conversion.

---

Happy converting!
