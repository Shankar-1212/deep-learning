# Photovoltaic Cell (PV) Segmentation Project
----
This project focuses on segmenting photovoltaic cells (PV) using two different models: DeepLabV3+ and YOLO. Additionally, utilized a Stable Diffusion pipeline to create augmented data for training the models.
## Models Used
- **DeepLabV3+**
- **YOLO**
## Data Augmentation
To enhance the dataset, we created augmented data using the Stable Diffusion pipeline. This augmentation helped improve the model's performance on the validation set. 
Both DeepLabV3+ and YOLO models were trained on both the original and augmented datasets. The results of the initial experiments are summarized in the table below.

## Results

| Model           | Training IoU | Validation IoU |
|-----------------|--------------|----------------|
| deeplab_non_aug | 0.98         | 0.94           |
| deeplab_aug     | 0.98         | 0.97           |
| yolo_non_aug    | 0.73         | 0.59           |
| yolo_aug        | 0.74         | 0.61           |

## Conclusion
The DeepLabV3+ model demonstrated superior performance compared to the YOLO model in segmenting photovoltaic cells, particularly when trained on augmented data. The use of data augmentation significantly improved the validation IoU for both models, with DeepLabV3+ achieving the highest validation IoU of 0.97.
