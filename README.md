# Dubai Satellite Imagery Segmentation (Beginner Version)

This project provides a **beginner-friendly workflow** for semantic segmentation of Dubai satellite imagery, using a simple UNet model with TensorFlow/Keras. It is intended for those new to deep learning, computer vision, or semantic segmentation.

## Features

- Clear, step-by-step Jupyter notebook (`Dubai_Segmentation_Basic.ipynb`)
- Loads satellite images and corresponding segmentation masks
- Converts mask colors to class indices based on `classes.json`
- Builds and trains a simple UNet model for multi-class segmentation
- Easily visualizes ground truth and predictions

## Folder Structure

```
Dubai-Segmentation-Basic/
├── Dubai_Segmentation_Basic.ipynb
├── classes.json
├── README.md
├── requirements.txt
├── data/
│   ├── Tile 1/
│   │   ├── images/
│   │   └── masks/
│   ├── Tile 2/
│   │   ├── images/
│   │   └── masks/
│   └── ... (more tiles if available)
```

- **Dubai_Segmentation_Basic.ipynb** – The main notebook
- **classes.json** – Class color definitions for the segmentation masks
- **requirements.txt** – Python dependencies
- **data/** – Folder for images and masks, structured as in the original dataset

## Data Source & Credits

All satellite imagery and annotated masks are from the excellent public dataset by [Ayush Dabra](https://huggingface.co/datasets/ayushdabra/dubai-satellite-imagery-segmentation):

- [ayushdabra/dubai-satellite-imagery-segmentation on HuggingFace](https://huggingface.co/datasets/ayushdabra/dubai-satellite-imagery-segmentation)

Please cite or credit the original author if you use this data in your own work.

## Quick Start

1. Download the dataset and extract it into the `data/` folder as shown above.
2. Place `classes.json` in the root directory.
3. Install requirements:  
   ```
   pip install -r requirements.txt
   ```
4. Open the notebook and run all cells.

---

## License

This code is MIT licensed. Please check the dataset page for its specific data license.