<p align="center"><img width="40%" src="dlami.png" /></p>

--------------------------------------------------------------------------------

**Latest update: we've renamed TFAMI to DLAMI to cover most deep learning frameworks**

## How to find?
Under community AMI, search for `DLAMI.V1`.

## DLAMI.V1 (latest stable AMI)
- Python 2.7
- PyTorch 0.1.12
- TensorFlow 1.0.1
- Theano 0.8.2
- Keras 1.2.2
- MXNet 0.9.3
- Lua 
- Torch
- CNTK
- Caffe
- CUDA release 7.5
- CuDNN 5.1


## FAQs (Relating to Driver Issues)
1. Error: `Failed to initialize NVML: Driver/library version mismatch`
	- Run `sudo reboot`. 
2. Error: `NVIDIA-SMI has failed because it couldn't communicate with the NVIDIA driver. Make sure that the latest NVIDIA driver is installed and running.`
	- Run `sudo apt-get update`.
3. Error: `Mismatch of Kernel with DSO`
	- Run `sudo reboot`.

## Regions (DLAMI.V1)
- Oregon `ami-7e3a5b1e`

## DLAMI Instance Specifications
- 50 GB EBS
- Can be used on any GPU instances including the new p2 instances.

## Have a bug to report?
Raise an issue here and we'll update DLAMI to make sure it works or enable it across different regions.

## Information
This is actively maintained by [Ritchie Ng](http://www.ritchieng.com/) from the National University of Singapore.

And I would like to thank Amazon for their donation of AWS credits for our research that led to this useful byproduct deployed by people across the world.

## License
MIT