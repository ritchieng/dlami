# TensorFlow AWS AMI aka TFAMI
Are you frustrated that many AMIs are not working to get TensorFlow working? Or that you have to waste time setting up your instances?

This is an AMI that I hope people, including myself, would continually monitor and ensure it works all the time. I call it TFAMI! How innovative.

Also, I have included Keras and OpenAI Gym as a bonus! Other packages can be easily installed with `pip install package_name` if you need anything else. 

## How to find?
Under community AMI, search for `TFAMI.v2` or `TFAMI`.

## TFAMI.v2 (latest stable AMI)
- Tensorflow 0.10.0
- Keras 1.1.0
- CUDA 8.0
- CuDNN 5.1
- Python 2.7
- Ubuntu 16.04

## TFAMI 
- TensorFlow 0.8.0
- Keras 1.0.4
- OpenAI Gym
- Python 2.7
- CUDA 7.5
- CuDNN 5
- Ubuntu 14.04

## How to install? 
If you are a unfamiliar with Amazon AWS GPU instance, I suggest you use this [guide](http://machinelearningmastery.com/develop-evaluate-large-deep-learning-models-keras-amazon-web-services/) that is made for beginners. Trust me, you cannot go wrong with the guide and this AMI! Instead of using the AMI that the website recommends (you will know when you reach that section how to search for an AMI), just search for `TFAMI.v2` or `TFAMI` instead. 

Please take note we have updated TensorFlow and all of its dependencies. The new version is available as `TFAMI.v2`. 

## Regions (TFAMI.v2)
- N. Virginia `ami-a96634be`
- Ohio `ami-73045e16`
- N. California `ami-813a71e1`
- Oregon `ami-ac8b2fcc`
- Singapore `ami-2c0bad4f`
- Ireland `ami-19d49a6a`
- Frankfurt `ami-155ca57a`
- Tokyo `ami-b701a7d6`
- Seoul `ami-80ec38ee`
- Sydney `ami-ec201d8f`
- Mumbai `ami-1b562274`
- Sao Paulo `ami-0c28b560`

## Regions (TFAMI)
- N. Virginia `ami-d0e4adc7`
- N. California `ami-5ce2ab3c`
- Oregon `ami-92af74f2`
- Singapore `ami-4362c520`
- Ireland `ami-b8f7b4cb`
- Frankfurt `ami-d09b65bf`
- Tokyo `ami-9331eaf2`
- Seoul `ami-45a3772b`
- Sydney `ami-be596bdd`
- Mumbai `ami-fe1a6e91`
- Sao Paulo `ami-cd2fbda1`

## TFAMI.v2 Instance Specifications
- 100 GB EBS
- Can be used on any GPU instances including the new p2 instances.
_You can easily change your EBS volume with this [guide](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-expand-volume.html)._

## TFAMI Instance Specifications
- 40 GB EBS
- Can be used on any GPU instances including the new p2 instances.

## Have a bug to report?
Raise an issue here and we'll update TFAMI to make sure it works or enable it across different regions.

## License
MIT