# 9517_CV_Proj
Group leader: Tianyu Li,   
Group members: Bingchen Qiu, Junliang Liu, Runmin Li, Ziyi Zhang   
(Sorted by the first letter of the first names)     

Introduction  
The goal of the group project is to work together to solve a computer vision problem and present solutions and results in both oral and written form. 
We use Computer vision methods to help to precisely segment crop from field images.

Dataset   
The public dataset to be used in this group project is available from EWS-Dataset.zip.
It contains 190 RGB images of 350 x 350 pixels with manual annotation in the form of binary masks for plants and soil

Methods   
Feature-based Pixel Classification + Random Forest by TTToo9(Runmin Li)  
K-means by peterqiu616(Bingchen Qiu)  
SAM by leoljom(Tianyu Li)   
Sam_zero-shot_val by Kayins2778(JunLiang Liu)  
Watershed by 2YULt1(Ziyi Zhang)  
(Sorted by the first letter of the method/algorithm)   

Finally,we simplified SAM to obtain sam_zero-shot_val to evaluate the segmentation capability of SAM.  
It was not trained or fine-tuned on the EWS-Dataset.  
Instead,it directly used the pre-trained weights and was evaluated on the validation set.  
The final running time was 1 minute and 41 seconds.

Most of the notebooks run based on libraries like opencv-python, numpy, matplotlib, scikit-learn.   
Notebook SAM.ipynb will besides use other libraries like PyTorch, garbage collect(gc). 
If you decide to run SAM.ipynb on your own local machine, please install Segment Anything first:
    "pip install git+https://github.com/facebookresearch/segment-anything.git"   
or clone the repository locally and install with:   
    "git clone git@github.com:facebookresearch/segment-anything.git   
    cd segment-anything; pip install -e ."   
Also, please download the corresponding checkpoint file of ViT model you choose.   
    ViT_H: https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth      
    ViT_L: https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth   
    ViT_B: https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth   
Otherwise, please follow the steps in the notebook if you are using Kaggle or Colab.  

