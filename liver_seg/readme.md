# Liver Segmentation Project
----
This project focuses on liver segmentation using two different models: ResNet-50 and MONAI. Below are the details and results of the experiments conducted with 

#### MONAI
- **Model Status:** Model Was Not Saved
- **Best Avg. Dice:** 0.947231113910675
- **Current Avg. Dice:** 0.9472296237945557

![MONAI Results](https://imgur.com/cvFAG3u.png)

#### ResNet-Training and Validation Metrics

| Epoch | Train Loss | Valid Loss | Foreground Accuracy | Custom Foreground Accuracy | Time  |
|-------|------------|------------|---------------------|----------------------------|-------|
| 0     | 0.011309   | 0.226557   | 0.870495            | 0.995171                   | 06:46 |
| 1     | 0.007404   | 0.007705   | 0.965589            | 0.997371                   | 06:47 |
| 2     | 0.004592   | 0.022877   | 0.950214            | 0.997900                   | 06:48 |
| 3     | 0.003597   | 0.005290   | 0.964382            | 0.998304                   | 06:48 |
| 4     | 0.003087   | 0.008241   | 0.955415            | 0.998332                   | 06:46 |

![ResNet-50 Results](https://imgur.com/T0yNxwM.png)

#### Observations
- **Epoch 0:** Better model found with valid_loss value: 0.22655658423900604.
- **Epoch 1:** Better model found with valid_loss value: 0.007705126889050007.
- **Epoch 3:** Better model found with valid_loss value: 0.005289705004543066.

## Conclusion

Both models showed promising results for liver segmentation, with ResNet-50 achieving significant improvements in validation loss over epochs. MONAI achieved a high Avg—dice score.
