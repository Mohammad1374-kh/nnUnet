# nnUnet
The project for finetuning the nnU-net to do the segmentation of the medical images (nifty) of the MSD -medical segmentation decathlon- spleen data
The step-by-step guide is available in the Jupiter notebook
In case of getting Error in preprocessing the dataset by the command, use the following structure for the dataset:
1- The dataset should have three folders named imagesTr(training original nifty images) , labelsTr(segmentation in nifty format) , imagesTs(original nifty images for the test set) and a json file called dataset.json
2- The naming convention for the imagesTr and imagesTs convention is; organName_threeDigitsUniqeNumber_fourDigitsNumberSpecifyingModality.nii(.gz)
3- The labelTs folder have the same naming convention except for the last part (modality : CT or MRI) before the file extension(.nii) that should be removed for labels (segmentation images)
4- The datset.json structure can be checked in the relevant file
**note:  Except for the dataset, there is the ground truth labels file( real segmentation for the test images) that should be given to the model for the evaluation part.
