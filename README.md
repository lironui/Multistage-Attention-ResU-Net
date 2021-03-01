# Multistage-Attention-ResU-Net

In this repository, we re-factor the skip connections in the raw U-Net and design a Multi-stage Attention ResU-Net (MAResU-Net) for semantic segmentation from fine-resolution remote sensing images.

The detailed results can be seen in the [Multi-stage Attention ResU-Net for Semantic Segmentation of Fine-Resolution Remote Sensing Images](https://arxiv.org/ftp/arxiv/papers/2011/2011.14302.pdf).

The related repositories include:
* [MACU-Net](https://github.com/lironui/MACU-Net)->The code to train the network.
* [Linear-Attention-Mechanism](https://github.com/lironui/Linear-Attention-Mechanism)->The raw inplement of the LAM.

Feel free to contact me if you need any further information: lironui@163.com

If our code is helpful to you, please cite:

`Li, Rui, et al. "Multistage Attention ResU-Net for Semantic Segmentation of Fine-Resolution Remote Sensing Images." IEEE Geoscience and Remote Sensing Letters (2021): 1-5.`

Acknowlegement:
------- 
Thanks very much for the sincere help from Jianlin Su as well as his blog [线性Attention的探索：Attention必须有个Softmax吗？](https://spaces.ac.cn/archives/7546)


Requirements：
------- 
```
numpy >= 1.16.5
PyTorch >= 1.3.1
sklearn >= 0.20.4
tqdm >= 4.46.1
imageio >= 2.8.0
```

Network:
------- 
![network](https://github.com/lironui/MAResU-Net/blob/main/Fig/network.png)  
Fig. 1.  The structure of (a) the proposed MAResU-Net and (b) the attention block.

Result:
------- 
![Result](https://github.com/lironui/MAResU-Net/blob/main/Fig/network.png)  
Fig. 2. Visualization of results on the Vaihingen.

Complexity:
------- 
![Complexity](https://github.com/lironui/MAResU-Net/blob/main/Fig/complexity.png)  
Fig. 3. The (a) computation requirement and (b) memory requirement of the raw dot-product attention mechanism and the proposed linear attention mechanism under different input sizes. Please notice that the figure is in log scale.
