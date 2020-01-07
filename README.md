DTI_PROCESSING
==============

A general processing pipeline for diffusion data.

Please read the wiki pages for advice on how to get started.

Created by Kirstie Whitaker, on July 1st 2013.
Contact: kw401@cam.ac.uk


Revise 2020.01.07
==============
1. change bedpostx to bedpostx_gpu, it's about 100x faster than bedpostx


Environment
==============
* Hardware
    * RTX 2060
* Software
    * system: centos 7.6 64bit
    * Nvidia GPU driver: 440.44 (GPU compatible)
    * CUDA: 10.1 
    * fsl 6.0: https://fsl.fmrib.ox.ac.uk/fsldownloads_registration
    * bedpostx_gpu: for 6.x and cuda 10.1, https://users.fmrib.ox.ac.uk/~moisesf/Bedpostx_GPU/Installation.html
    * sudo yum install -y dos2unix
    * input "csh" to use command "setenv"
* Directory structure
    * Project dir
        * wrapper.sh
        * SCRIPTS
            * DTI_PROCESSING-master
                * files in this repository
        * SUB_DATA 
            * n001
                * DTI
                    * dti.nii.gz
                    * bvals
                    * bvecs_orig
                * MPRAGE
                    * center_of_mass
                    * highres.nii.gz
            * n002

RUN
=============
```bash
./wrapper.sh
```
            
