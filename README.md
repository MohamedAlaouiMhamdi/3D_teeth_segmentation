# 3D Teeth Segmentation using PointNet

## Table of Contents
- [Introduction](#introduction)
- [Model Architecture](#model-architecture)
- [Dataset](#dataset)
- [Results](#results)
- [Future Work](#future-work)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Introduction
**3D Teeth Segmentation using PointNet** is an advanced deep learning project designed to automate the segmentation of teeth from 3D dental scans. Leveraging the power of PointNet—a neural network architecture specifically crafted for handling point cloud data—this project addresses the challenges associated with accurate and efficient dental segmentation. Precise segmentation is crucial for various dental applications, including orthodontic planning, prosthodontics, and oral surgery, thereby enhancing both diagnostic capabilities and treatment outcomes.

## Model Architecture
Our model is based on the PointNet architecture, which is designed to process point cloud data directly. The key components of our architecture include:

1. **Input Transformation**: A mini-network that aligns the input points to a canonical space.
2. **Feature Transformation**: Another mini-network that aligns features to a canonical space.
3. **Segmentation Network**: A series of multi-layer perceptrons (MLPs) that extract global and local features.
4. **Output Layer**: A final layer that predicts the segmentation label for each point.
5. 
<img width="383" alt="Screenshot 2024-09-24 155927" src="https://github.com/user-attachments/assets/2fea936f-ac82-4867-bfdc-867394156998">

The model's ability to handle unordered point sets makes it particularly suitable for 3D dental scans, where the number and order of points can vary between scans.

## Dataset
Our model was trained and evaluated on a proprietary dataset of 3D dental scans, consisting of:
- 300 high-resolution 3D scans of full dental arches

## Results
<img width="425" alt="Screenshot 2024-09-24 160011" src="https://github.com/user-attachments/assets/4f6e272c-31db-40c2-8c7e-3ef4f653aa41">

<img width="464" alt="Screenshot 2024-09-24 155950" src="https://github.com/user-attachments/assets/4f64382c-737c-4c1a-9280-db92229eae06">


### Visualization of Results

#### True vs. Predicted Segmentation
![True vs. Predicted Segmentation](https://github.com/user-attachments/assets/a8ab6ccb-f6f7-4b1d-ab6a-8ee1b1fe5ce4)
*Figure 1: Comparison of True vs. Predicted Teeth Segmentation*

This visualization demonstrates the high accuracy of our model in segmenting individual teeth from a full 3D dental scan. The left image shows the ground truth segmentation, while the right image displays our model's predictions. Note the precise delineation of tooth boundaries and the correct identification of different tooth types.

### Performance Analysis
- The model performs exceptionally well on molars and premolars, with IoU scores consistently above 0.94.
- Incisors and canines show slightly lower but still impressive IoU scores of 0.89-0.91.
- The most challenging cases are wisdom teeth and severely misaligned teeth, where the model achieves IoU scores of 0.85-0.88.

## Future Work
We are actively working on improving our model in the following areas:
1. Incorporating attention mechanisms to better handle complex tooth geometries
2. Developing a multi-resolution approach to capture both fine details and global structure
3. Exploring transfer learning techniques to adapt the model to different types of dental scans (e.g., CT, CBCT)

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgements
- **PointNet Authors**: [Qi et al., 2017](https://arxiv.org/abs/1612.00593)
- **Open3D**: For their excellent library on 3D data processing.
- **3D Smart Factory**: For supervision and guidance.

## Contact
**Mohamed Alaoui Mhamdi**
- **Email**: al.mh.mohamed@gmail.com
- **LinkedIn**: [MohamedalaouiMhamdi](https://www.linkedin.com/in/alaoui-mhamdi-mohamed/)
- **GitHub**: [mohamedAlaouimhamdi](https://github.com/MohamedAlaouiMhamdi)

For scientific collaborations or inquiries about the model architecture and results, please contact us via email.
