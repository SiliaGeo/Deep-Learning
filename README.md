American Sign Language Recognition

Dataset Overview (Uploaded on Kaggle)

This project focuses on the recognition of American Sign Language (ASL) using a 27 Classes Dataset. The dataset is carefully curated with essential information for data preprocessing, ensuring a deep understanding of its format and characteristics. The following details are extracted from the dataset creators' paper:

    Volunteers: Data collected from 173 volunteers.
    Hand Used: Signs are shaped using the right hand.
    Classes:
        Numbers (Static Gestures): 0, 1, 2, 3, 4, 5, 6, 7, 8, 9.
        Letters (Static Gestures): A, B, C, D, E.
        Expressions (Dynamic Gestures): Hello, Yes, No, Good, Bye, Good morning, Pardon, Project, Little bit, Please, What’s up.
        NULL Class: 314 images without any gesture and with a different background.
    Image Capture: RGB camera with a 3024 x 3024 pixel frame size.
    Image Size: 128 x 128 pixels.
    Normalization: Images are normalized.
    Data Split: 130 images taken from each person, 5 from each class.
    Total Images: 22,801.
    Data Representation: Processed images stored in a numpy Tensor ‘X’ with 4 dimensions (number of images, image height, image width, RGB channels).
    Labels: Numpy Tensor ‘Y’ created containing labels of the images with 2 dimensions (number of images, 1), where each image corresponds to one label.

Data Processing

    One-Hot Encoding: Applied to the labels for categorical representation.
    Data Augmentation: Techniques used to increase the diversity of the dataset, enhancing model robustness.

Convolutional Neural Network (CNN)

A Convolutional Neural Network was employed for the recognition task, leveraging the spatial hierarchy present in the images. The architecture was designed to effectively capture and learn intricate features from the ASL gestures.
