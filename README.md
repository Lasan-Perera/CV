# Computer Vision & Machine Vision

Coursework, notes, and experiments for my university CV/Machine Vision module.

## Setup

```bash
git clone https://github.com/Lasan-Perera/CV.git
cd CV
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

System packages (Ubuntu) needed for OpenCV windows:

```bash
sudo apt install -y libgl1 libglib2.0-0 ffmpeg
```

## Structure

```
CV/
├── notebooks/   # Jupyter notebooks — theory and exercises
├── scripts/     # Standalone .py scripts (webcam, cv2.imshow demos)
├── data/
│   ├── images/  # Test images (not tracked)
│   └── videos/
├── output/      # Generated results (not tracked)
└── notes/       # Written notes and summaries
```

## Notes

- Notebooks use `matplotlib` for display — `cv2.imshow()` misbehaves in Jupyter.
- OpenCV loads images as **BGR**; convert with `cv2.cvtColor(img, cv2.COLOR_BGR2RGB)` before plotting.
- Always check `if img is None:` after `cv2.imread()` — it fails silently on bad paths.
- `data/` and `output/` are gitignored; add your own test images locally.


## Environment

Ubuntu · Python 3 · OpenCV 5.0 · VS Code
