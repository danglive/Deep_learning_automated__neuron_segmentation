# CREMIchallenge2017\ Neuron Image Segmentation Task
Tentative experiments of electron microscopy neuron images: Neuron Segmentation Task. (see at: https://cremi.org, see leaderboard at: https://cremi.org/leaderboard/)


##### Nueron Boundary Prediction task, statistical restuls and visualization: 
(with ~acc inception: 98.68%, augmented 98.88%):

<img src="https://raw.githubusercontent.com/celisun/CREMIchallenge2017_segmentation_task/master/loss.png" width="500">
<img src="https://raw.githubusercontent.com/celisun/CREMIchallenge2017_segmentation_task/master/acc.png" width="500">
<img src="https://github.com/celisun/cremi/blob/master/6p.png" width="600">

##### Approaches: 
  - Used residual network method. original: https://arxiv.org/abs/1512.03385, implementation on github: https://github.com/gcr/torch-residual-networks
  - Only green and purple area will be selected in minibatches, dilated boundary yellow area will be avoided.
  - Different random rotation techniques. In my experiment, rand+/-60 to 50% of samples in each batch performs the best.
<img src="https://raw.githubusercontent.com/celisun/CREMIchallenge2017_segmentation_task/master/*Filtered%20Mask.png" width="600">
<img src="https://raw.githubusercontent.com/celisun/CREMIchallenge2017_segmentation_task/master/*Visualize%20Boundary.png" width="600">
<img src="https://raw.githubusercontent.com/celisun/CREMIchallenge2017_segmentation_task/master/rot.png" width="600">



