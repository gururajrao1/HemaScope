HemaScope — Blood Cell Detection & Annotation Pipeline
Overview

HemaScope is a Python-based pipeline designed for preprocessing and visualizing microscopic blood cell images from the BCCD dataset. This project handles the parsing of XML annotations, dataset splitting, cell cropping, annotation format conversion, mask generation, and statistical counting of blood cell types — all essential steps to prep your data for machine learning tasks in hematology and biomedical imaging.
Features

    Visualizes annotated bounding boxes for White Blood Cells (WBC), Red Blood Cells (RBC), and Platelets.

    Splits dataset into training, validation, and testing sets with customizable ratios.

    Crops individual blood cells from full-slide images based on bounding box coordinates.

    Converts Pascal VOC XML annotations to YOLO format text files for object detection models.

    Generates segmentation masks outlining each blood cell for advanced analysis.

    Produces CSV reports summarizing counts of different cell types per image.

Getting Started
Prerequisites

    Python 3.7 or above

    Required packages: xmltodict, Pillow, matplotlib

Install dependencies with:

pip install xmltodict Pillow matplotlib

Setup

    Clone this repository:

git clone <your_repo_url>
cd HemaScope

    Download the BCCD dataset and place it in the project directory.

    Run the scripts to:

        Visualize sample images with annotations

        Split the dataset into train/val/test folders

        Crop individual cell images

        Convert annotations to YOLO format

        Generate segmentation masks

        Create CSV summary of cell counts

(You can find the scripts and instructions in the scripts/ folder.)
Usage

python visualize_annotations.py
python split_dataset.py
python crop_cells.py
python convert_to_yolo.py
python generate_masks.py
python generate_counts.py

(Adjust filenames as per your setup.)
Contributing

Feel free to open issues or submit pull requests to improve the pipeline or add new features!
License

This project is licensed under the MIT License.
