# Heat Diffusion PINN with Amazon Q

This is a tiny experiment built using **Amazon Q** inside **Amazon CodeCatalyst** to quickly prototype a **Physics-Informed Neural Network (PINN)** that solves the **Heat equation**.

Instead of training on data, the model learns by minimizing the residual of the heat equation itself. The neural network takes space and time as input and predicts temperature, and the training loop enforces the physics rule using automatic differentiation.

## What Amazon Q Did
- Generated the base neural network architecture in **PyTorch**  
- Wrote the training loop and autograd-based derivative code  
- Helped create a quick plot of the learned temperature profile  
- Drafted a snippet to upload the results to **Amazon S3** using **boto3**

## How to Run
1. Open this notebook in **Google Colab**  
2. Install dependencies and run all cells  
3. After training, view the temperature plot and optionally upload it to your S3 bucket

## Notes
This was built in about an hour as a fast demo of how Amazon Q can speed up early-stage scientific ML prototyping by handling boilerplate, letting you focus on core model logic.
