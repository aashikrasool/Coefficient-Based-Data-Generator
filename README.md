# Synthetic Data Generation using GANs with Self-Attention and Correlation Constraint

## Overview
This project aims to generate synthetic data that closely resembles real-world data using Generative Adversarial Networks (GANs). In this implementation, we utilize a custom self-attention layer and introduce a correlation constraint to ensure that the generated data preserves the correlation structure of the real data.


## Dataset
In this work we utilized crop production recomendation data which is publically available in Kaggle[1].

## Implementation Details
### Synthetic Data Generation
- **GAN Architecture**:
- ![Archictecture](https://github.com/aashikrasool/Coefficient-Based-Data-Generator/blob/main/GAN%20arch.png)
- Our framework introduces a multi-head attention layer within the generator. This innovation allows for a more nuanced discernment and emphasis on critical inter-feature relationships in tabular data, significantly improving the model's capability to capture and replicate complex data dynamics in the agricultural domain.


### Training
- **Data Splitting**: Explain how the real data is split into training and test sets.
- **Correlation Calculation**: Describe how the correlation coefficient is calculated from the training data.
- **GAN Training**: Detail the training procedure for the GAN model, including the number of epochs, batch size, and optimization techniques used.

### Evaluation
- **Correlation Analysis**: Explain how the correlation between the generated and real data is evaluated after training the GAN model.
- **Results**: Present the correlation coefficient between the real and synthetic data and discuss the performance of the model.

## Usage
Provide instructions on how to use the code to generate synthetic data. Include code snippets or commands for running the training script and generating synthetic data.

## Example
Show an example of how to generate synthetic data using the provided code. Include sample input and output data.

## License
Specify the license under which the code is released.

## Acknowledgments
Acknowledge any contributions, libraries, or datasets used in the project.

## References
[1] https://www.kaggle.com/datasets/aksahaha/crop-recommendation

