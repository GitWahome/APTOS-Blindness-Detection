# APTOS-Blindness-Detection
Fetched From:
https://www.kaggle.com/c/aptos2019-blindness-detection/overview

Given the size of the image files. you may need to download the files from here:
https://www.kaggle.com/c/aptos2019-blindness-detection/data
before running the kernel.

Imagine being able to detect blindness before it happened.

Millions of people suffer from diabetic retinopathy, the leading cause of blindness among working aged adults. Aravind Eye Hospital in India hopes to detect and prevent this disease among people living in rural areas where medical screening is difficult to conduct. Successful entries in this competition will improve the hospital’s ability to identify potential patients. Further, the solutions will be spread to other Ophthalmologists through the 4th Asia Pacific Tele-Ophthalmology Society (APTOS) Symposium

Currently, Aravind technicians travel to these rural areas to capture images and then rely on highly trained doctors to review the images and provide diagnosis. Their goal is to scale their efforts through technology; to gain the ability to automatically screen images for disease and provide information on how severe the condition may be.

In this synchronous Kernels-only competition, you'll build a machine learning model to speed up disease detection. You’ll work with thousands of images collected in rural areas to help identify diabetic retinopathy automatically. If successful, you will not only help to prevent lifelong blindness, but these models may be used to detect other sorts of diseases in the future, like glaucoma and macular degeneration.

## General Approach: I make use of multiple Quick and dirty implementations of SVCs, a single layer Neural Network and Logistic regression as voters. The class predicted is either the modal class or in case of ties, the class predicted byt the single most accurate of the models.

Some image preprocessing has been done to make the algorithm work better. So far, the best performance I have gotten our of a single run has been 79.6% with 99% variance explained and the image dimentions 400px by 400px. This version of the Kernel achieves less accuracy and runs much faster. Most of the runs consistently hit 75%+

I will be implementing a refined Neural Network for the same using tensor flow .
This is an example of the preloaded images and their respective categories. In this example the images are already inverted and the black spots more visible due to the kernelized contrast modification. This is what has allowed such a quick and dirty implementtation using Scikit to perform commendably well.

![alt text](https://i.postimg.cc/mkWHjRkz/Screen-Shot-2019-07-26-at-11-54-02-PM.png)

