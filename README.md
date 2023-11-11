# TYJTDet
This method performs 3D object detection in the BEV space using images from multiple cameras. It first predicts the depth of each camera and then projects the extracted image features into BEV space. Moreover, it utilizes temporal information by aligning the BEV features. We use single model flip test time augmentation.

## Results
### 3D Object Detection (on nuScenes test)

|   Model   | mAP  | NDS  |
| :-------: | :--: | :--: |
| TYJTDet-swin |54.45 | 52.12 |
| TYJTDet-vov99|60.28 | 67.50 |


## Get Started

### Environment
This implementation is build upon [mmdetection3d](https://github.com/open-mmlab/mmdetection3d), please follow the steps in [install.md](./docs/install.md) to prepare the environment.

### Data
Please follow the official instructions of mmdetection3d to process the nuScenes dataset.(https://mmdetection3d.readthedocs.io/en/latest/datasets/nuscenes_det.html)


## Acknowledgement
Many thanks to the following open-source projects:
* [mmdetection3d](https://github.com/open-mmlab/mmdetection3d)
*  [SparseBEV](https://github.com/MCG-NJU/SparseBEV)

## Reference

```bibtex
@{author={Zhengmi, Zoujian, Zhenhua Guo}}
```
