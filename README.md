# DCaps
Tensorflow 2 implementation for D-Caps: Diagnosis Capsules

## Requirements

The model contains the following libraries and frameworks
- Tensorflow 2.4

## Useful Links:
- Paper- "Dynamic Routing Between Capsules": [Link](https://papers.nips.cc/paper/2017/file/2cad8fa47bbef282badbb8de5374b894-Paper.pdf)
- Paper "DIAGNOSING COLORECTAL POLYPS IN THE WILD WITH CAPSULE NETWORKS": [arXiV](https://arxiv.org/pdf/2001.03305.pdf)<br />Paper by Rodney LaLonde, Pujan Kandel, Concetto Spampinato, Michael B. Wallace, and Ulas Bagci.
- Blog Tutorial: [Link](https://rodneylalonde.wixsite.com/personal/post/d-caps-diagnosis-capsules)
- GitHub reference: [Link](https://github.com/lalonderodney/D-Caps)

**Note:** <br />The implementation is not completed without the last pooling layer and the reconstruction part<br />

**Note:** <br />The implementation is quite different<br />
- I changed some naming styles
- I embedded the routing inside the ConvCapsuleLayer
- The routing is nearly the same with some little modifications
- I used different squash function and it's also inside the ConvCapsuleLayer
- If using Binary Classifications (2 classes) the shape of the last layer will be different because of the tf.squeeze()

![Full D-Caps](https://github.com/MoGomaa/DCaps/blob/main/FullDCaps.png)
