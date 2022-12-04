# Deformable DETR JAX Porting Faithfullness Check

This is a hacked version of Deformable DETR that can be used to test the faithfullness of its JAX port.

## Notable Changes

* Force padding to 1333.
* Use tensorflow jpeg decoder.
* Use tensorflow resize in data pipeline.
* Use nearest-exact when resizeing padding masks.
* Copy resnet.py to help debugging.