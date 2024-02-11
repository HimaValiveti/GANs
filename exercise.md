# Image Generation using GANs
## Learning Outcomes

* Understanding the basic components in Generative Adversarial Networks and their working principles
* Diving into the process of Image Generation with GANs
* Implementing GAN architectures using tensor flow and keras libraries
* Evaluate and strategically choose activation functions to enhance the performance of the model
* Addressing the challenges and Ethical and Societal concerns offered by the GANs
  

**Generative Adversarial Networks (GANs)**, a class of Generative-AI are modelled by pairing opposing neural networks **Generator** and **Discriminator**, extract and represent complex features of audio, image and video samples. 

The **Generator** endeavours to generate artificial images that are indistinguishable from original. 

The **Discriminator** determines the authentication of the counterfeit image generated 

**Adversarial training** is the core principle. GANs employ a learning setup with a loss function in the form of the discriminator's feedback. This function helps the generator learn and generate realistic images without explicitly labeled data. The discriminator acts as a supervisor by continuously providing feedback to the generator, guiding it to craft images.
<center>
<img src="https://github.com/HimaValiveti/images/blob/main/Image1.JPG" width="500" height="300"> </center>

## Diving into the process of Image Generation with GANs

* A random noise vector (often distributed as Uniform or Gaussian) is given as input to the generator that manifests into mimic of the original image post several layers of computation. 

* Discriminator analyses both the original (from training data) and counterfeit image (image received from generator) and calculates the gradient (loss) and directs it to the generator for further training.
  
* The discriminator's output (predicted label) classifies the probability of input image as original or fake. It is a continuous value ranging between 0 and 1. A value around 1, indicates the input image is highly likely to be real and fake if the label is closer to 0.

## Learning Process

* The gradient signal information is back propagated to the generator. Hyperparameters are updated in the direction of minimizing the error.
  
* This iterative adversarial training procedure updates the weights and biases of both the networks and substantially enhances the network performance.
  
* The generator masters in deception and the discriminator in identifying the counterfeit imagery.

* This learning process continues until the generator generates indistinguishable images
  
## Implementation

Basic libraries,
<center><img src="https://github.com/HimaValiveti/images/blob/main/code_libraries.jpg" width="400" height="50"> </center>

The generator consists of three dense layers wherein the output dense layer has the activation function **tanh** which produces 28X28(784) dimensional vector for every image input within the normalized range [-1,1].  This vector is forwarded to the discriminator which flattens the 28X28 vector. Activation functions, **ReLU** are used for faster convergence of the generator/discriminator models and **Sigmoid** is used for depicting the originality of image.

<center><img src="https://github.com/HimaValiveti/images/blob/main/discriptive_Model.jpg" width="400" height="200"> </center>

<center><img src="https://github.com/HimaValiveti/images/blob/main/generative_model_1.jpg" width="500" height="300"> </center>

Furthermore, the discriminator and generator are trained and the hyperparameters are updated according to the learning environment.

## Limitations
 
**Mode collapse:** Generator fails to completely learn the distribution of the sample data and generates samples that lack diversity- **Generator overfitting**

**Vanishing Gradient:** Discriminator feeds back negligible gradient to the generator, hampering the updation of hyperparameters and slowing down the learning process- **Discriminator overfitting**

### Ethical Concerns
* Wrongly used Deepfake videos and audios of individuals propel frauds and harm people
* Mimicking the literature developed by humans indirectly violating their Intellectual Property Rights
* The generated output can be prejudiced if the training data is not sensitized

## Conclusion

Over the past decade GAN models have been constantly evolving making them suitable for a plethora of computing applications. Higher quality of the training data and learning the model for a longer duration ensure that the generated data outperforms the original. Furthermore, imposing ethical guidelines and eliminating sensitive data can help mitigate the ethical concerns to a major extent.

## References

1. Bok, V., & Langr, J. (2019). GANs in Action: Deep learning with Generative Adversarial Networks. Simon and Schuster.
2. Porkodi, S. P., Sarada, V., Maik, V., & Gurushankar, K. (2023). Generic image application using GANs (generative adversarial networks): a review. Evolving Systems, 14(5), 903-917. 
3. Dash, A., Ye, J., & Wang, G. (2023). A review of Generative Adversarial Networks (GANs) and its applications in a wide variety of disciplines: From Medical to Remote Sensing. IEEE Access.
4. Saxena, D., & Cao, J. (2021). Generative adversarial networks (GANs) challenges, solutions, and future directions. ACM Computing Surveys (CSUR), 54(3), 1-42.
5. Sun, Y., Wu, Z., Ma, Y., & Tresp, V. (2024). Quantum Architecture Search with Unsupervised Representation Learning. arXiv preprint arXiv:2401.11576.

## Assessment
1. The core objective of generator in GANs is?
    *	To differentiate real and counterfeit images
    *	To generate counterfeit images that mimic training data
    *	To minimize the gradient
    *	To categorize real and counterfeit images
2. Discriminator is majorly responsible for
    *	To differentiate real and counterfeit images
    *	To generate counterfeit images that mimic training data
    *	To minimize the gradient
    *	To categorize real and counterfeit images
3. Binary classification is used for discriminating the real and fake images 
    *	True
    *	False
4. The limitations of GANs are 
    *	Overfitting of the training data
    *	Training instability
    *	Ethical concerns related to deepfake content
    *	All of the above
5. The network architecture/s commonly used in GANs is
    *	Random Forest
    *	Multilayer perceptrons
    *	Conventional Neural Networks
    *	Recurrent Neural Networks

