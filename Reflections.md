## Reflections

* Surveyed thoroughly the literature available on GANs over the last decade and related the concept of neural network to GANs as the reader is acquainted with the same
* The literature referred contains journal and conference papers, open video content and Generative AI tools like ChatGPT and Google Gemini
* Listed keywords based on which the content can be conceptualized
* Leveraged AI tools to get a direction/structure of the content
* Provided only a few code snippets from the implementation because of word limit
* Learning outcomes were prepared according to the Blooms Taxonamy levels
* GAN is unsupervised learning model and explicitly differentiating it with supervised models would help the learner understand labelled and unlabelled data. I wanted to start by differentiating the descriptive and generative models but thought that I would be digressing away from the main topic of interest.
* GANs are implemented on the principles of Deep neural networks where higher level of abstraction is plausible. I wasn’t sure if GANs can think exactly like humans as there are contradictory remarks in literature reviewed and hence removed this statement.
* Inspite of the underlying limitations related to Ethical usage and balancing the Generator and Discriminator, GANs are used for a multitude of applications statement has been removed as the advanced models like cycle GAN were successful in acquiring stability.
* Focus on architectures (U-Net) used in GANs would have made the reader understand the advancements in improved learning rate and faster convergence but could not delve into because of the word limitation on the article.
* Sustainability of GANs was subtly included in the conclusion in order to stick to the word limit.
* Deleted the Classification of GANs and the related Learning outcome to adhere to the word limit. Please find the work below
### Learning Outcome: Evaluate and strategically choose GAN models applicable for diverse real-world scenarios

### Different types of GAN models and their applications in Image Generation

|Model | Prominent Features     | Applications       |
|---- | ------------ | ------------|
|Vanilla GAN **(2014)**	|Simple GAN with generator and discriminator pairing	|Image generation|
|Conditional GAN **(2015)**	|Labels and Texts appended for guided generation of images	| <li> Image Translation</li> <li>Text to Image tasks</li> |
|Deep Convolutional GANs **(2015)**	|Exploits the core principles of CNN	| <li> Landscape</li> <li>Monet</li> <li> Facial generation</li>|
|Wasserstein GANs **(2017)**	|Loss function is tabulated based on Wasserstein distance to enhance the stability of the duo	|Generating complex images|
|Style Transfer GANs **(2015)**	|Pre trained models are used  for feature extraction from images	|<li>Image manipulation </li><li>Artistic exploration </li>|
|Progressive GANs **(2018)**	|Start with images having low resolution during training, upsampling (generator) and downsampling (discrimator), Better stability|High resolution artistry|
|StyleGAN **(2019)**	|ProGAN	|Realistic and Diverse Facial generation|
|BigGAN **(2019)**		|ProGAN	|Large scale Image generation|
|Diffusion Models **(2020)**	|non-GAN model	|Text-to-image generation, image editing and manipulation|


