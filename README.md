MUSICAL
====


# Example results  

<img src="./results/paris_results/10_input.png" width="200">  <img src="./results/paris_results/10_ours.png" width="200">  <img src="./results/paris_results/66_input.png" width="200">  <img src="./results/paris_results/66_ours.png" width="200">
<img src="./results/celeba_results/5_input.png" width="200">  <img src="./results/celeba_results/5_ours.png" width="200">  <img src="./results/celeba_results/3_input.png" width="200">  <img src="./results/celeba_results/3_ours.png" width="200">
<img src="./results/places2_results/9_input.png" width="200">  <img src="./results/places2_results/9_ours.png" width="200">  <img src="./results/places2_results/5_input.png" width="200">  <img src="./results/places2_results/5_ours.png" width="200">

Example inpainting results of our method on images of building (Paris StreetView), face (CelebA), and natural scenes (Places2) with center masks (masks shown in gray). For each group, the masked input image is shown left, followed by sampled results from our model withour any post-processing.

# Getting started
## Training
* python train.py --name paris_parallel --CA_type parallel

## Testing
* python test.py --results_dir ./results_paris/ --name paris_parallel --CA_type parallel --checkpoints_dir ./log/paris_parallel --which_epoch 30 

## GUI
* python -m visdom.server

## Citation
If you use this code for your research, please cite our paper.

@inproceedings{wang2019musical,
  title     = {MUSICAL: Multi-Scale Image Contextual Attention Learning for Inpainting},
  author    = {Wang, Ning and Li, Jingyuan and Zhang, Lefei and Du, Bo},
  booktitle = {Proceedings of the Twenty-Eighth International Joint Conference on
               Artificial Intelligence, {IJCAI-19}},            
  pages     = {3748--3754},
  year      = {2019}
}
