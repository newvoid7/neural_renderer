# Neural 3D Mesh Renderer

This repo is the minor fixed version of neural-renderer-pytorch forked from [PyTorch implementation of the paper Neural 3D Mesh Renderer](https://github.com/daniilidis-group/neural_renderer). The original paper is [Neural Mesh Renderer](hiroharu-kato.com/projects_en/neural_renderer.html). 

## Updates
1. Updated the version number in setup.py.
2. Modified the `./cuda/*.cpp` by adding the AT_CHECK macro.
3. Added the atomicAdd function in `./cuda/rasterize_cuda_kernel.cu`.
4. Added the "up" parameter in look.py and look_at.py, also changed the renderer.py.
5. Updated the [::-1] operation by using flip method in rasterize.py.

## Requirements
Python 3.6+ and PyTorch 1.8.0+, gcc 5.0+ (support C++11). Tested on Python 3.9 and PyTorch 1.10.1 as well.

## Installation
You can install the package by running
```
python setup.py install
```
Since running install.py requires PyTorch, make sure to install PyTorch before running the above command.

## Citation

```
@InProceedings{kato2018renderer
    title={Neural 3D Mesh Renderer},
    author={Kato, Hiroharu and Ushiku, Yoshitaka and Harada, Tatsuya},
    booktitle={The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
    year={2018}
}
```
