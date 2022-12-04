# Deformable DETR JAX Porting Faithfullness Check

This is a hacked version of [Deformable DETR](https://github.com/fundamentalvision/Deformable-DETR) that can be used to test the faithfullness of its [JAX port](https://github.com/google-research/scenic/tree/main/scenic/projects/baselines/deformable_detr).

## Notable Changes

* Force padding to 1333.
* Use tensorflow jpeg decoder.
* Use tensorflow resize in data pipeline.
* Use nearest-exact when resizeing padding masks.
* Copy resnet.py to help debugging.