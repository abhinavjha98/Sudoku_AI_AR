# Sudoku-py

An augmented reality sudoku solver using OpenCV.

## Usage

### Installation
>pip install -r requirements.txt

### main.py
```
usage: main.py [-h] [-f FILE] [-s] [-w] [-d]

arguments:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  File path to an image of a sudoku puzzle
  -s, --save            Save image to specified file's current directory
  -w, --webcam          Use webcam to solve sudoku puzzle in real time
                        (EXPERIMENTAL)
  -d, --debug           Enables debug information output
```

## Examples
>python main.py --file assets/c6.jpg



>python main.py --webcam





## Limitations
- Webcam solver cannot detect when a new puzzle has entered the frame, will try to warp the solution of the first puzzle it sees onto any subsequent puzzles
- OCR predictions are very spotty for hand written digits and stylized fonts
- Cannot solve puzzles that don't have a distinguishable four-point outer border
