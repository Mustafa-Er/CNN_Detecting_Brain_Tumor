# CNN_Detecting_Brain_Tumor

🧠 Brain Tumor Detection from MRI Images
This project aims to detect the presence of brain tumors from MRI images using deep learning techniques and transfer learning with three powerful convolutional neural network (CNN) architectures.

📁 Dataset Overview
The dataset contains MRI images labeled as:

Yes (tumor present)

No (no tumor)

The data is split into:

Training Set

Validation Set

Test Set

🛠 Preprocessing Steps
Label Distribution Check:
Counted the number of 'yes' and 'no' labeled images across all dataset splits to verify class balance.

Cropping:
All MRI images were cropped to focus on the brain region and remove unnecessary background.

Data Augmentation:
Applied real-time augmentation using ImageDataGenerator to improve model generalization.
Techniques included:

Rotation

Zoom

Horizontal and vertical flips

Shearing, etc.

🤖 Models Used
Three pre-trained CNN architectures were fine-tuned on the processed dataset:

1. VGG16


  Accuracy: 0.80

  Precision: 0.75

  Recall: 0.90

  F1 Score: 0.82



2. ResNet50


  Accuracy: 0.75
  
  Precision: 0.69
  
  Recall: 0.90
  
  F1 Score: 0.78

3. InceptionV3

  Accuracy: 0.85
  
  Precision: 0.77
  
  Recall: 1.00
  
  F1 Score: 0.87


✅ Best Model
Based on evaluation on the test set, InceptionV3 achieved the best overall performance, especially with a perfect recall of 1.00, making it highly effective at detecting tumors without missing cases.

📌 Conclusion
This project demonstrates how transfer learning can be leveraged for medical image classification. Preprocessing steps like cropping and augmentation, combined with powerful CNN models, can yield strong performance in tumor detection tasks.
