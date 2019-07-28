# kaggle_SteelDefectDetection
Code repository for Kaggle Steel Defect Detection Competition


## target:
For each image you must segment defects of each class (ClassId = [1, 2, 3, 4]), and caculate DICE score for each defect class as accuracy. 

## Our Method 
* Coarse-to-Fine
  [tab] * step 1: Detection network to propose possible image regions(coarse);
  [tab] * step 2: Based on step 1, pixel-wise segementation to achieve fine-grained;
  [tab] * step 3: Find most effective Ensemble models； 
  [tab] * step 4: [Optional] Using traditional ML algorithm to propagate and restore the boundory；


* WE don't rely on single segmentation network
[tab][tab]* GPU hardware demanding during large image training;   
[tab][tab]* redundant computation on normal region should be reduced;
[tab][tab]* 


### stage-0: naive version(Week 1)

####(a) Segmentation Network: FCN

[tab][tab][tab]* pre-prosessing

[tab][tab][tab]* model && parameter

[tab][tab][tab]* fine-tuning

[tab][tab][tab]* train/test result




####(b) Detection Network: + Segmentation Network: FCN

[tab][tab][tab]* pre-prosessing

[tab][tab][tab]* model && parameter

[tab][tab][tab]* fine-tuning

[tab][tab][tab]* train/test result






