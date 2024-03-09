# Synthetic Data Generation using GANs with Self-Attention and Correlation Constraint

## Overview
This project aims to generate synthetic data that closely resembles real-world data using Generative Adversarial Networks (GANs). In this implementation, we utilize a custom self-attention layer and introduce a correlation constraint to ensure that the generated data preserves the correlation structure of the real data.


## Dataset
In this work we utilized crop production recomendation data which is publically available in Kaggle[1].

## Implementation Details
### Synthetic Data Generation
 **GAN Architecture**:
 
- ![Archictecture](https://github.com/aashikrasool/Coefficient-Based-Data-Generator/blob/main/GAN%20arch.png)
- Our framework introduces a multi-head attention layer within the generator. This innovation allows for a more nuanced discernment and emphasis on critical inter-feature relationships in tabular data, significantly improving the model's capability to capture and replicate complex data dynamics in the agricultural domain.



### Evaluation
- Though the labels 'pH' and 'Temperature' show almost 95% probability distribution, the number of each label is dramatically various. Moreover, it is the limitation of tabular GANs that they are not able to generate a specific amount of data. Nevertheless, our proposed approach performs better in producing evenly distributed data that closely resembles the original data in all columns with a likeness of 98%, except for the 'P' (Phosphorus) column, where the synthetic data shows a more rapid increase initially, suggesting a higher density of lower values compared to real data .
- ![ResultAnalysis](https://github.com/aashikrasool/Coefficient-Based-Data-Generator/blob/main/performance.png)



## License
This work is licensed under the Custom Collaborative License. Any modification or redistribution of this work requires explicit permission from all collaborators listed in the acknowledgments section of this README file. For inquiries about modifications or collaborations, please contact the project maintainers.

## Acknowledgments

We would like to acknowledge the contributions of the following individuals from the Data Centric AI class:

- M.J. Aashik Rasool
- Abrar Alabdulwahab
- Sevara Mardieva
- Dong Seok Kim

They implemented the approach described in this project.

## References
[1] https://www.kaggle.com/datasets/aksahaha/crop-recommendation

