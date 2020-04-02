# SAGAN-For-WSI-Segmentation

I have implemented SAGAN model based on [Han Zhang et al.](https://arxiv.org/pdf/1805.08318.pdf)
For the generator I have used a U-Net architecture with ResNet. 
The WSI (Whole Slide Images) used for training and testing the model were used from the the paper written by [Brendon et al.](https://www.nature.com/articles/s42256-019-0018-3)

The results obtained for Mouse Kidney cells for a 4 class problem are as follows:

|               | Precision   | Recall | F1 Score | IOU    |
|:-------------:|:-----------:|:------:|:--------:|:------:|
| Glomeruli     | 0.9916      | 0.9876 | 0.9896   | 0.9795 |
| Nuclei        | 0.97        | 0.9516 | 0.9607   | 0.9244 |
| Non-Nuclei    | 0.9579      | 0.9568 | 0.9574   | 0.9182 |
| Background    | 0.9955      | 0.9983 | 0.9969   | 0.9939 |
| Overall       | 0.9788      | 0.9736 | 0.9762   | 0.954  |
