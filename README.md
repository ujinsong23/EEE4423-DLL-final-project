_The project took place in May - June 2023._
# Out of distribution Detection method for a MNIST classification


The Out-of-Distribution (OOD) detection in an MNIST classifier model operates as follows: Initially, a classifier is trained using only labeled images of digits '1' to '9'. Subsequently, when images containing the digit '0' are introduced, the trained classifier is expected to accurately determine whether the given image belongs to the in-distribution or out-of-distribution category. The `Report.pdf` begins by briefly summarizing relevant previous works related to OOD detection _(Section 2)_ and then provides detailed explanations of the model's architecture and algorithm _(Section 3)_. Following this, experimental results are presented _(Section 4)_, along with several ablation studies to demonstrate the contributions of each component of the designed model to its performance.

`Model.ipynb` contains the complete programming of the project, covering aspects such as model design, training, and validation. By simultaneously training a denoising autoencoder and a classifier model for in-distribution data and incorporating loss functions to balance the probability for incorrect predictions, the model successfully identified unfamiliar data during the validation process.

![alt text](https://github.com/ujinsong23/EEE4423-DLL-final-project/blob/main/Figures/Architecture.jpg)

The `weights` folder includes various model weights, with `final_weight.pt` being one of the best-performing weights that yielded superior quantitative results.
