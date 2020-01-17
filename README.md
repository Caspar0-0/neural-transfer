# Neural Style Transfer
This paper reviews neural style transfer applications from several aspects. This paper asks and answers questions such as how does change in parameters of representations based on a pre-trained convolutional neural network affect the visual results in synthesized images. Three content images and three different style images selected to generate nine blended images for comparison. The 19-layer VGG network model serves as the primary framework for this analysis. Modifications to the original implementation such as adjusting learning rates, exploring different initializing image, changing training iterations, experimenting different random seeds, and attempting relative weights of content and style loss in the loss function help observe the blended image difference, etc. The results from trial and error will be discussed and explained to reach conclusion and further research suggestions.
## Model
According to the original paper, 5 layers are used to extract style features, containing 'conv1_1', 'conv2_1', 'conv3_1', 'conv4_1', 'conv5_1';  'conv4_2' layer is used to extract content features.

## Procedure
Run the content image through the VGG19 model and compute the content cost

Run the style through the VGG19 model and compute the style cost 

Compute the total cost

Define the optimizer and the learning rate, and then run gradient descent algorithm
