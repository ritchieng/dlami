<p align="center"><img width="40%" src="tfami.png" /></p>

--------------------------------------------------------------------------------
Are you frustrated that many AMIs are not working to get TensorFlow working? Or that you have to waste time setting up your instances?

This is an AMI that I hope people, including myself, would continually monitor and ensure it works all the time. I call it TFAMI! How innovative.

It comes with some packages pre-installed like Python, Keras and TensorLayer. Other packages can be easily installed with `pip install package_name` if you need anything else. 

## How to find?
Under community AMI, search for `TFAMI.v3`.

## TFAMI.v3 (latest stable AMI)
_This works on both `p2` and `g2` instances._
- Tensorflow 0.12 [head](https://github.com/tensorflow/tensorflow/tree/9d66dae6fc5d1b964a03498ddabb97a78a999015)
- Keras 1.1.0
- TensorLayer 1.2.7
- CUDA 8.0
- CuDNN 5.1
- Python 2.7
- Ubuntu 16.04

## TFAMI.v2 (old)
_If you are running `p2 instance`, you should use this._
- Tensorflow 0.10.0
- Keras 1.1.0
- CUDA 8.0
- CuDNN 5.1
- Python 2.7
- Ubuntu 16.04

## TFAMI (old)
_If you are running `g2 instance`, you should use this._
- TensorFlow 0.8.0
- Keras 1.0.4
- OpenAI Gym
- Python 2.7
- CUDA 7.5
- CuDNN 5
- Ubuntu 14.04

## How to install? 
If you are a unfamiliar with Amazon AWS GPU instance, I suggest you use this [guide](http://machinelearningmastery.com/develop-evaluate-large-deep-learning-models-keras-amazon-web-services/) that is made for beginners. Trust me, you cannot go wrong with the guide and this AMI! Instead of using the AMI that the website recommends (you will know when you reach that section how to search for an AMI), just search for `TFAMI.v3`.

Please take note we have updated TensorFlow and all of its dependencies. The new version is available as `TFAMI.v3`. 

## FAQs (Relating to Driver Issues)
1. Error: `Failed to initialize NVML: Driver/library version mismatch`
	- Run `sudo reboot`. 
2. Error: `NVIDIA-SMI has failed because it couldn't communicate with the NVIDIA driver. Make sure that the latest NVIDIA driver is installed and running.`
	- Run `sudo apt-get update`.
3. Why does `p2 instance` work with only `TFAMI.v2`. 
	- This is due to a configuration I did when I manually compiled TensorFlow and indicated `compute capability 3.5` where `g2 instance` only has `compute capability 3.0`.
	- Both `g2 instance` and `p2 instance` would work on the official `TFAMI.v3`. 
4. Error: `Mismatch of Kernel with DSO`
	- Run `sudo reboot`.

## Regions (TFAMI.v3)
- N. Virginia `ami-0e969619`
- Ohio `ami-9cc69cf9`
- N. California `ami-08451468`
- Oregon `ami-52bb0c32`
- Canada `ami-cb2694af`
- Singapore `ami-2c0bad4f`
- Ireland `ami-b34566c0`
- Frankfurt `ami-515c9c3e`
- London `ami-d4e2e8b0`
- Singapore `ami-e6862885`
- Sydney `ami-baa19ad9`
- Seoul `ami-8fa87ee1`
- Tokyo `ami-96e982f1`
- Mumbai `ami-3fcdba50`
- Sao Paulo `ami-19198175`


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

## TFAMI.v3 Instance Specifications
- 100 GB EBS
- Can be used on any GPU instances including the new p2 instances and the old g2 instances
_You can easily change your EBS volume with this [guide](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-expand-volume.html)._

## TFAMI.v2 Instance Specifications
- 100 GB EBS
- Can be used only with g2 instances due to `compute capability 3.5`
_You can easily change your EBS volume with this [guide](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-expand-volume.html)._

## TFAMI Instance Specifications
- 40 GB EBS
- Can be used on any GPU instances including the new p2 instances.

## Have a bug to report?
Raise an issue here and we'll update TFAMI to make sure it works or enable it across different regions.

## Information
This is actively maintained by [Ritchie Ng](http://www.ritchieng.com/) from the National University of Singapore.

And I would like to thank Amazon for their donation of AWS credits for our research that led to this useful byproduct deployed by people across the world.

## Upcoming Updates
- TensorFlow 1.0.0
- All dependencies updated accordingly.
	- Keras
	- TensorLayer
	- CUDA
	- CuDNN

## License
MIT