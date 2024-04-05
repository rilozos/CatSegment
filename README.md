# CatSegment: Cat Segmentation Model for Snapchat Lens

This project develops a cat segmentation model using MobileNetV2, implemented in PyTorch and utilizing the Torchvision library. Designed specifically for Snap Inc as part of an externship, this model leverages the COCO dataset to accurately segment cats in images, enabling the creation of engaging Snapchat Lenses.

![download](https://github.com/rilozos/CatSegment/assets/112525112/6edeb7c8-b397-4265-bd61-90ef81828c93)

## Project Overview

The aim of this project is to provide a lightweight yet efficient segmentation model capable of identifying and segmenting cats within a wide range of environments and poses. By employing MobileNetV2, the model achieves a balance between accuracy and performance, making it suitable for real-time applications in Snapchat Lenses. A key component in the development and training of this model was leveraging cloud-based resources. Specifically, I used [Brev.dev](https://www.brev.dev/) to create and manage a GPU instance in the cloud, utilizing Lambda Labs GPU cloud with NVIDIA A100 GPUs. This setup allowed us to significantly accelerate the training process, showcasing the efficiency and scalability that cloud computing brings to AI and machine learning projects. This solution enabled me to easily access GPU's on the cloud to train the model rapidly, saving an incredible amount of time.

## Features

- Utilizes the efficient MobileNetV2 architecture for fast, accurate segmentation.
- Trained on the COCO dataset for robust detection capabilities across diverse scenarios.
- Integrated with PyTorch and Torchvision for industry standard computer vision technologies.
- Customizable for further refinement and training on additional classes within COCO.

## References

This project builds upon several key resources and datasets:

- The training approach and integration with Snapchat Lenses leverage the [Snapchat SnapML Templates](https://github.com/Snapchat/snapml-templates/blob/main/Custom%20Segmentation/segmentation_training.ipynb). This resource provides a foundational understanding of creating custom segmentation models specifically for Snapchat Lens Studio. It's important to note that additional installations and dependenciy changes were required due to deprecations, and the notebook has been modified to train a custom model on a different section of the COCO dataset.
- The COCO dataset, which is a large-scale object detection, segmentation, and captioning dataset, is utilized for training the segmentation model. More information about the COCO dataset can be found on its official website: [COCO dataset](http://cocodataset.org/).
- [Brev.dev](https://www.brev.dev/) was instrumental in facilitating the development and training process. Utilizing Brev.dev's tools, a GPU instance in the cloud was created using Lambda Labs GPU cloud, leveraging NVIDIA A100 GPUs. This setup significantly accelerated the training process, demonstrating the power and flexibility of cloud-based development environments for AI and machine learning projects.
