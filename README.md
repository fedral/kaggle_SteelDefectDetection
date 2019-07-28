# kaggle_SteelDefectDetection
Code repository for Kaggle Steel Defect Detection Competition


## target:
For each image you must segment defects of each class (ClassId = [1, 2, 3, 4]), and caculate DICE score for each defect class as accuracy. 

## Our Method 
* Coarse-to-Fine
	* step 1: Detection network to propose possible image regions(coarse);
	* step 2: Based on step 1, pixel-wise segementation to achieve fine-grained;
	* step 3: Find most effective Ensemble models； 
	* step 4: [Optional] Using traditional ML algorithm to propagate and restore the boundory；


* WE don't rely on single segmentation network
	'''- GPU hardware demanding during large image training;'''diff   
	'''- Redundant computation on normal region should be reduced;'''diff
		 




## stage-0: naive version(Week 1)

###  Data pre-processing:
		SV-Image conversion + Data augmentation 

#### (a) Segmentation Network: FCN

#### (b) Detection Network: Mask RCNN + Segmentation Network: FCN








