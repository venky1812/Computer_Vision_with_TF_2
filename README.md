# Computer_Vision_with_TF_2
## Image Classification :
In layperson’s terms, image classification answers the question: “what object does this image contain?” More specifically, “This image contains X object with what probability,”.
### Image Classification pipeline:

  1) Load an image.
  
  2) Resize it to a predefined size such as 224 x 224 pixels.
  
  3) Scale the values of the pixel to the range [0,1] or [–1,1], a.k.a. normalization.
  
  4) Select a pretrained model.
  
  5) Run the pretrained model on the image to get a list of category predictions and their respective probabilities.
  
  6) Display a few of the highest probability categories.
  
 ##### Point to remember:
  Heatmaps are a great way to visually detect bias in the data. The quality of a model’s predictions depends heavily on the data on which it was trained. If the data is biased, that will reflect in the predictions.
  
  As we collect data, we must be vigilant at the outset of potential bias that can pollute our model’s learning. For example, when collecting images to build a food classifier, we should verify that the other artifacts such as plates and utensils are not being learned as food. Otherwise, the presence of chopsticks might get our food classified as chow mein. Another term to define this is co-occurrence. Food very frequently co-occurs with cutlery. So watch out for these artifacts seeping into your classifier’s training.
  
  Useful tools for neural network visualization : Keras-vis,tf_explain.
  
## Transfer Learning:

  • 
  
  • The complexity and power of what a layer can recognize increases as we approach the final layers. Conversely, the reusability of a layer decreases as we get closer to the  
    output. 
    
  • The decision on how many layers to fine tune is dependent on the amount of data at hand as well as the similarity of the target task to the original dataset on which the 
    pretrained model was trained.
