# Task 1

## 20k
![20k final image](./Images/20kFinal.png)
![20k evolution](./Images/20k.gif)
![20k loss](./Images/20k.PNG)

## 100k
![100k final image](./Images/100kFinal.png)
![100k evolution](./Images/100k.gif)
![100k loss](./Images/100k.PNG)

## GAN improvments

From [Soumith Chintala 2016](https://www.youtube.com/watch?v=myGAju4L7O8)

- Nomalize inputs between -1, 1 and use tanh as output layer in generator
- Modify loss function max log D instead of min log 1-D
- Use spherical noise vector 
- Don't mix generated data with real data (batch norm)
- Avoid sparse gradients, replace relu and maxpool with leakyrelu and average pooling for example
- Label smoothing, predict with probabilities of being in class
- Use DCGANs when able to
