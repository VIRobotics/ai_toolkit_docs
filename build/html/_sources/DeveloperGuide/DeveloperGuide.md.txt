# Developer Guide

## Introduction

This chapter aims to help developers fully understand and proficiently use the **AI Vision Toolkit for OpenVINO (AIVT-OV)**. Through the content of this chapter, you will learn how to quickly get started, master basic operations, use advanced features, troubleshoot common issues, and optimize performance, ensuring that you can efficiently develop and deploy applications based on AIVT-OV.

By reading this chapter, you will learn:

- **Creating and Configuring Projects**: Create new projects from scratch and properly configure the necessary environment and dependencies.
- **Using Basic Functions**: Master the basic functions and operations of the AIVT-OV toolkit to perform simple image processing and visual recognition tasks.
- **Using Advanced Features**: Understand and use the advanced features of the toolkit to perform complex deep learning and computer vision tasks.
- **Troubleshooting**: Identify and resolve common issues and errors encountered during development.
- **Deploying Applications**: Learn how to deploy developed applications to target devices and optimize performance and hardware configurations.

## Quick Start

### Function Introduction

The installed OpenVINO toolkit can be found in Block Diagram >> Functions >> Addons >> VIRobotics >> AI Vision Toolkit for OpenVINO, including the `opencv_yiku`, `OpenVINO`, and `ModelZoo` modules.

<img src="..\_static\imgs\DeveloperGuide\fuctions.png" alt="functions" style="zoom:100%;" />

Here are the detailed introductions of these three modules:

1. opencv_yiku
   - Supports easy image acquisition using mainstream USB cameras and network cameras, with high-speed image acquisition.
   - Provides hundreds of traditional image processing operators in OpenCV to meet various needs, such as image filtering, morphology operations, feature detection, and template matching.
   - Suitable for basic image processing and preprocessing tasks.
2. OpenVINO
   - Integrates OpenVINO™'s deep learning inference engine functions, supporting the loading and running of various deep learning models.
   - Supports multiple hardware acceleration options (such as CPU, GPU, VPU) to optimize inference performance.
3. ModelZoo
   - Includes functions for deep learning model loading and inference, which can be used for image classification, object detection, and image segmentation tasks.
   - Provides convenient model loading and configuration interfaces to help developers quickly apply models.

### Example Guide

Examples can be found in the `LabVIEW install path\examples\VIRobotics\AI Vision\` directory. They can also be found in LabVIEW help: Help >> Find Examples >> Directory Structure >> VIRobotics >> AI Vision

<img src="..\_static\imgs\DeveloperGuide\find_examples.png" />

These examples are mainly divided into the following four parts:

1. CV
   - Includes examples of traditional vision processing content, such as edge detection, morphology operations, filtering, etc.
   - Examples: `Edge Detection.vi`, `Morphological Operations.vi`
2. License Management
   - Mainly used for activation examples during deployment.
   - Examples: `Activate License.vi`, `Check License Status.vi`
3. Object Detection
   - Mainly YOLO series object detection examples, including models such as YOLOv5/YOLOv6/YOLOv7/YOLOv8 Seg/YOLOv8 Pose/YOLOv8 OBB, etc.
4. Segment
   - Includes segmentation examples of DeepLabv3/DeepLabv3+ and yiku-seg.

Each example provides detailed step-by-step instructions and annotations to help developers understand and apply these features.

## Troubleshooting

### Common Issues and Solutions

- Issue 1: Toolkit Installation Failed
  - Solution: Ensure all security software is disabled and VIPM is run as an administrator.
- Issue 2: Unable to Activate License
  - Solution: Verify that the License ID and Key are entered correctly and check the network connection. If necessary, contact technical support for assistance.
- Issue 3: Camera Not Connecting
  - Solution: Ensure the camera is properly connected to the computer and the driver is correctly installed. Try changing the USB port or restarting the computer.

### Error Codes and Their Meanings

To be updated...

## Deployment

To be updated...

## FAQ

- **Question 1: How do I check my license status?**
  - Answer: Open LabVIEW, click Tools—VIRobotics License Manager, and check the license status.
- **Question 2: How do I update the toolkit to the latest version?**
  - Answer: Use VIPM to search for the latest version of the AIVT-OV toolkit and install it. Ensure all security software is disabled and run VIPM as an administrator.
- **Question 3: My image processing speed is slow. How can I optimize it?**
  - Answer: Ensure hardware acceleration options are enabled, optimize image processing algorithms, and reduce unnecessary computational steps.

If you have any other questions, please contact the technical support team at support@virobotics.net.