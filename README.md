# TensorFlow AWS AMI aka TFAMI
Are you frustrated that many AMIs are not working to get TensorFlow working? Or that you have to waste time setting up your instances?

This is an AMI that I hope people, including myself, would continually monitor and ensure it works all the time. I call it TFAMI! How innovative.

Also, I have included Keras and OpenAI Gym as a bonus! You can do most of your work. Other packages are easily installed with pip if you need anything else. 

## How to find?
Under community AMI, search for TFAMI.

## Cool Stuff Installed and Ready to Use
- TensorFlow 0.8.0
- Keras 1.0.4
- OpenAI Gym
- Python 2.7
- CUDA 7.5
- CuDNN 5

## How to install? 
If you are a complete noob with Amazon AWS GPU instance, I suggest you use this [guide](http://machinelearningmastery.com/develop-evaluate-large-deep-learning-models-keras-amazon-web-services/) that is for beginners. Trust me, you cannot go wrong with the guide and this AMI! Instead of using the AMI that the website recommends (you will know when you reach that section how to search for an AMI), just search for TFAMI instead. 

## Instance Specifications
- 40 GB EBS
- Can be used on any GPU instances including the new p2 instances.

## Actively Tested Regions
- N. Virginia `ami-d0e4adc7`
- N. California `ami-5ce2ab3c`
- Oregon `ami-92af74f2`
- Singapore `ami-4362c520`


## All Other Regions
- Ireland `ami-b8f7b4cb`
- Frankfurt `ami-d09b65bf`
- Tokyo `ami-9331eaf2`
- Seoul `ami-45a3772b`
- Sydney `ami-be596bdd`
- Mumbai `ami-fe1a6e91`
- Sao Paulo `ami-cd2fbda1`


## Have a bug to report?
Raise an issue here and we'll update TFAMI to make sure it works or enable it across different regions.

## License
Open source of course! Check the MIT license in the repository.