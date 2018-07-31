# Generative Image 

[CVPR 2018 Paper](https://arxiv.org/abs/1801.07892) | [ArXiv](https://arxiv.org/abs/1801.07892) | [Project](http://jiahuiyu.com/deepfill) | [Demo](http://jiahuiyu.com/deepfill) | [YouTube](https://youtu.be/xz1ZvcdhgQ0) | [BibTex](#citing)

**Update (Jun, 2018)**:
1. The tech report of our new image inpainting system DeepFillv2 is released. [ArXiv](http://arxiv.org/abs/1806.03589) | [Project](http://jiahuiyu.com/deepfill2)
2. We also released recorded demo video [YouTube](https://youtu.be/xz1ZvcdhgQ0) based on DeepFillv1 (CVPR 2018), as well as video [YouTube](https://youtu.be/uZkEi9Y2dj4) of DeepFillv2. Best viewed with highest resolution 1080p.
3. DeepFillv1 is trained and mainly works on rectangular masks, while DeepFillv2 can complete images on free-form masks with user guidance as an option.


<img src="https://github.com/katychou/generative01/blob/master/examples/001.jpg" width="425"/> <img src="https://github.com/katychou/generative01/blob/master/examples/output01.png" width="425"/>


Example inpainting results of our method on images of natural scene (Places2), face (CelebA) and object (ImageNet). Missing regions are shown in white. In each pair, the left is input image and right is the direct output of our trained generative neural networks without any post-processing.

## Run

Testing:
    * Run `python test.py --image examples/input.png --mask examples/mask.png --output examples/output.png --checkpoint model_logs/your_model_dir`.


## TensorBoard

Visualization on [TensorBoard](https://www.tensorflow.org/programmers_guide/summaries_and_tensorboard) for training and validation is supported. Run `tensorboard --logdir model_logs --port 6006` to view training progress.

