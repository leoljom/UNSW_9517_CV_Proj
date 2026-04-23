# 9517_CV_Proj

(Sort by the first letter of the method/algorithm)  
Feature-based Pixel Classification + Random Forest by TTToo9(Runmin Li)  
K-means by peterqiu616(Bingchen Qiu)  
SAM by leoljom(Tianyu Li)  
Watershed by 2YULt1(Ziyi Zhang)  

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
