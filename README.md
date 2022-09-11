# ESRGAN

ESRGAN = *Enhanced Super Resolution Generative Adversarial Network* for IVUS Images

Based on the repository by [Kuan-Yu Huang](https://github.com/peteryuX/esrgan-tf2)


## Data Preparation
- by executing 'data/convert_train_tfrecord.py'
- Code:
	**python data/convert_train_tfrecord.py 
					--output_path="./data/DIV2K800_sub_bin.tfrecord" 
					--is_binary=True**
- add other arguments if required

## Training
- by executing 'train_esrgan.py'
- Code: 
	**python train_esrgan.py 
	--cfg_path="./configs/esrgan.yaml" 
	--gpu=1**
- add other arguments if required


## Testing
- by executing 'train_esrgan.py'
- Code: 
	**python test.py 
	--cfg_path="./configs/esrgan.yaml" 
	--img_path PATH**
- add other arguments if required


## Execution
- upload ESRGAN.ipynb file to Google Colaboratory
- follow instructions
- execute elements in the order they are included


## File Structure
- **ESRGAN.ipynb**: Google Colaboratory execution file
- **train_esrgan.py**: training function
- **test.py**: testing function
- **configs**: includes the ESRGAN configuration file
- **data**: function to prepare the dataset
- **modules**: some additional functions
- **SRImages**: some example images generated with the ESRGAN models and LR input images
- **pretrainedModel**: pre-trained model utilized for transfer learning
- no trained models could be uploaded due to the high file size


