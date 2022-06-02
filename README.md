# big_data_fmri


### Content


#### Searchlight implementation and spark comparison


*Searchlight_roi_fMRI_classification.ipynb* Implementation of searchlight algorithm in python and comparison with spark/no spark



#### Classification based on entire image data


*beta_image_classification.ipynb* Reads in fMRI data (which is not in this repo) and performs classification on raw whole brain images and brain subregions. 
Output are the classification scores :

subj02_svm_result_log ...

subj07_svm_result_log ...



*fMRI_data_evaluation_ajp.ipynb* Reads and analyses the result files porduced by classification script.



*output_mask.nii* : The mask containing brain regions. It's a 3D matrix of the same size as the individual timepoint images and each voxel has a value corresponding to its brain region (based on brainnetome atlas, we just picked one, but could of course try and compare different masks)


### To-Do list

Goal : Classify data(beta images) to labels (0,1)

    1) Use entire images as vector & run classification [Alex] (check)
    2) Select specific voxels (ROIs) or searchlight (sphere around a voxel) [Claire] (check)
    3) Move to spark (failed)
    4) Expand to more patients (check)
    5) Improve models
    6) Write paper
    7) Get nobel prize
    8) Sleep (check)
    

