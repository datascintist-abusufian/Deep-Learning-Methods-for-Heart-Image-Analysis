# Deep Learning Methods for Heart Image Analysis

A comparison of classical and deep-learning approaches to cardiac MRI analysis. The project covers segmentation (thresholding, region-based, watershed and edge detection) and a hybrid model that combines a CNN, an autoencoder and an RNN.

## Data

| Data | Source | In repo |
| --- | --- | --- |
| Cardiac MRI volumes (Task02_Heart) | [Medical Segmentation Decathlon](http://medicaldecathlon.com/), King's College London | No (download separately) |
| 2D cardiac MRI slices with labels | [Roboflow heart-segmentation-2](https://universe.roboflow.com/memoire/heart-segmentation-2/dataset/1), CC BY 4.0 | `heart_dataset.zip` |

The data are documented in `Revised Proper Dataset Documentation.pdf`.

## Notebooks

| Notebook | Purpose |
| --- | --- |
| `MRI_Heart_Image_data__Preprocessing_sufi.ipynb` | Preprocessing and classical segmentation: Otsu and adaptive thresholding, region-based methods, watershed, Canny edges, augmentation |
| `MRI_image_data__24_10-2023_diverge algorithm.ipynb` | An alternative run of the same segmentation pipeline |
| `CNN+AE+RNN_sufi.ipynb` | Hybrid deep-learning model (CNN, autoencoder and RNN) with augmentation and evaluation |
| `sensitivity_analysis_on_parameters.ipynb` | Sensitivity of results to key parameters |

## Running it

```bash
pip install tensorflow nibabel opencv-python scikit-image scikit-learn matplotlib seaborn
```

The notebooks were written in Google Colab with Google Drive mounted. Change the data paths to run them locally.

## Licence

No licence has been declared yet. Each dataset keeps its own licence.

## Author

Md Abu Sufian - ORCID [0009-0007-3503-6942](https://orcid.org/0009-0007-3503-6942)
