# Chinese Digits Classification
## Problem statement: A Chinese spin on the classic MNIST problem where the aim is to classify correctly chinese characters into their respective values

The digits stand for 0 to 9, followed by 10, 100, 1000 and 10,000.
![chinese mnist](https://github.com/user-attachments/assets/152ba40a-a963-4100-88bd-6ee60abf5d94)

## Dataset
Size: 15000 rows (12000 train, 1500 test, 1500 validation)
resolution: Each image is 64 x 64 pixels, in grayscale. Each of the 4096 pixels is a column itself in the dataset.

![Screenshot 2025-06-09 at 10 27 29 AM](https://github.com/user-attachments/assets/176b717f-b38c-4950-9c62-b3cd0ac20f70)

![Model 1 acc](https://github.com/user-attachments/assets/f4b6c333-500e-4012-ae8c-38eb0eb3f510)

![Model 1 loss](https://github.com/user-attachments/assets/17a5cdc1-1bc9-41c3-a2c0-af37673a30b9)

L1, L2 regularization (to address overfitting)
Dropout layers (good)
Early stopping

Final model selected: Model6
![Model_Comparison](https://github.com/user-attachments/assets/c2716c95-39bd-4fe5-89bc-f83e52084edf)


There were some characters that are more prone to be misclassified. From the visualization below, it looks like the label '11', aka the chinese numeral 千 is the character that is misclassified the most, as well as the label '12' aka 万. The only character that has the fewest incorrect predictions is the chinese character 一, or the number 1 (which is not surprising)

![Wrong Classification](https://github.com/user-attachments/assets/67126019-bcfc-4595-a583-e78cc4dfa260)


