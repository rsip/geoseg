# Geoseg - A Computer Vision Package for Automatic Building Segmentation and Outline extraction

## Structure of directories
### sub directories
```
Geoseg:
  ├── dataset/
  │   └── train, validate and test dataset
  ├── logs/
  │   ├── learning curve, logging, statistic, etc.
  ├── models/
  │   ├── fcn, fpn, u-net, segnet, etc.
  ├── result/
  │   └── quantitative & qualitative result
  ├── utils/
  │   ├── datasets.py
  │   ├── metrics.py
  │   ├── preprocess.py
  │   ├── runner.py
  │   └── vision.py
  │  
  ├── FCNs.py
  ├── FPN.py
  ├── UNet.py
  ├── MC-FCN.py
  ├── BR-Net.py
  ├── ResUNet.py
...
```
### Files for generate visualization
```
├── visSingle.py
├── visSingleComparison.py
...
```

## Model Performance

### Performance
* Overall accuracy, precision, recall, f1-score, jaccard index(IoU) and kappa coefficient
![performance](./result/excel/performance.png)

### Computational efficiency
* Train and Test FPS
![time](./result/excel/computational-efficiency.png)

## Visualization Samples

### Learning Curve
* FCN8s
![FCN8s training curve](./logs/curve/FCN8s_iter_5000.png)

### Segmentation and outline extraction
* FCN8s
![FCN8s segmentation maps](./result/single/FCN8s_canny_segmap_edge_1.png)

### Segmentation result comparison
* FCN32s, FCN16s, FCN8s
![FCN8s, FCN16s, FCN32s](./result/single-comparison/segmap_FCN32s_FCN16s_FCN8s_1.png)

### Edge extraction result comparison
* FCN32s, FCN16s, FCN8s
![FCN8s, FCN16s, FCN32s](./result/single-comparison/edge_FCN32s_FCN16s_FCN8s_1.png)


# Citation
If it helps, please cite the paper.
```
@article{wu2018geoseg,
  title={Geoseg: A Computer Vision Package for Automatic Building Segmentation and Outline Extraction},
  author={Wu, Guangming and Guo, Zhiling},
  journal={arXiv preprint arXiv:1809.03175},
  year={2018}
}
```