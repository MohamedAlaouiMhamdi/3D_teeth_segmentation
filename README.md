# 3D Teeth Segmentation using PointNet


## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Results](#results)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Introduction

**3D Teeth Segmentation using PointNet** is an advanced deep learning project designed to automate the segmentation of teeth from 3D dental scans. Leveraging the power of PointNet—a neural network architecture specifically crafted for handling point cloud data—this project addresses the challenges associated with accurate and efficient dental segmentation. Precise segmentation is crucial for various dental applications, including orthodontic planning, prosthodontics, and oral surgery, thereby enhancing both diagnostic capabilities and treatment outcomes.

![Sample Segmentation](path/to/sample_segmentation.png)

## Features

- **Direct Point Cloud Processing**: Utilizes PointNet to handle raw 3D point cloud data without the need for voxelization, preserving geometric integrity.
- **Advanced Data Preprocessing**: Implements noise reduction, normalization, and data augmentation techniques to enhance data quality and model robustness.
- **High-Accuracy Segmentation**: Achieves superior segmentation performance through optimized model architecture and training strategies.
- **Comprehensive Evaluation**: Incorporates both quantitative metrics and qualitative visualizations to assess model effectiveness.
- **Error Analysis**: Identifies common segmentation errors, providing insights for future improvements.



### Description

The dataset comprises 3D dental scans obtained from Cone Beam Computed Tomography (CBCT) machines. Each scan is represented as a point cloud with XYZ coordinates and associated labels for different dental structures, enabling precise segmentation tasks.

## Results


*Table 1: Performance Metrics of the PointNet Model*


#### True vs. Predicted Segmentation

<img width="770" alt="Screenshot 2024-09-24 154427" src="https://github.com/user-attachments/assets/a8ab6ccb-f6f7-4b1d-ab6a-8ee1b1fe5ce4">

*Figure 1: Comparison of True vs. Predicted Teeth Segmentation*




### Error Analysis

The model occasionally misclassifies adjacent teeth with similar geometrical features and struggles with areas having low point density due to occlusions or scanning limitations. These errors highlight the need for enhanced local feature capture and more diverse training data.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- **PointNet Authors**: [Qi et al., 2017](https://arxiv.org/abs/1612.00593)
- **Open3D**: For their excellent library on 3D data processing.
- **Euro Mediterranean University of Fez**: For providing the platform and resources to undertake this project.
- **3D Smart Factory**: For supervision and guidance.
- **Any Additional Contributors**: [List any individuals or organizations that contributed]

## Contact

**Mohamed Alaoui Mhamdi**

- **Email**: (al.mh.mohamed@gmail.com)
- **LinkedIn**: [MohamedalaouiMhamdi](https://www.linkedin.com/in/alaoui-mhamdi-mohamed/)
- **GitHub**: [mohamedAlaouimhamdi](https://github.com/MohamedAlaouiMhamdi)



