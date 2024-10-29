# Video-to-Audio

This project provides a straightforward tool to convert video files to audio. Built using Python, it leverages popular libraries to handle video processing, allowing users to extract audio from any video file format.

## Features

- **Convert Videos to Audio**: Supports multiple video formats and extracts audio efficiently.
- **Simple and Easy to Use**: Minimal setup required, with just a few lines of code needed to execute the conversion.
- **Customizable**: Easily modify to support additional formats or integrate into larger projects.

## Requirements

- **Python 3.x**
- **FFmpeg**: This library is required to handle the video processing. You can download it [here](https://ffmpeg.org/download.html).
- **MoviePy**: This Python module makes video processing simple and is essential for this project.

Install dependencies with:
```bash
pip install moviepy
```

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/RadwanJunior/Video-to-Audio.git
    cd Video-to-Audio
    ```

2. Place the video file in the project directory.

3. Run the script:
    ```bash
    python video_to_audio.py
    ```

4. The audio file will be generated in the same directory as an `.mp3` file.

## Code Walkthrough

1. **Importing Libraries**: The script uses `MoviePy` to load and process the video.
2. **Loading Video File**: The video file is loaded, and a method to extract audio is called.
3. **Exporting Audio**: The extracted audio is saved as an MP3 file in the project directory.

## Example

For example, to convert a video called `sample.mp4`:

```python
from moviepy.editor import VideoFileClip

clip = VideoFileClip("sample.mp4")
clip.audio.write_audiofile("output.mp3")
```

## Future Enhancements

- Support for batch conversions.
- Adding support for additional audio formats (e.g., `.wav`, `.aac`).
