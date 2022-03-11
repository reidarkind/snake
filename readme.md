# Snake game from CV Zone

This more or less a copy of the code from this project: [https://www.computervision.zone/courses/snake-game/](https://www.computervision.zone/courses/snake-game/)

I've added an environment file, some comments, printouts and keypress `q` for quitting and `p` for pause.

## Create environment

From project folder, run:

```bash
conda env create
```

Then activate

```bash
conda activate py310_snake
```

## Start

As you normally do, with

```bash
python main.py
```

Follow info in cmd prompt window:

```bash
Starting...
Found cam
Starting game. r=Restart when game over, p=pause, q=quit
```

## Setup

### Cam to use

Might need to change the integer in this code line:

```python
cap = cv2.VideoCapture(1, cv2.CAP_DSHOW)
```

to

```python
cap = cv2.VideoCapture(0, cv2.CAP_DSHOW)
```

if you have only one web cam.

### Cam resolution

Might need to comment out/ change these code lines according to your cam resolution:

```python
#original resolution
#cap.set(3, 1280)
#cap.set(4, 720)

# cam resolution
cap.set(3, 1920)
cap.set(4, 1080)
```
