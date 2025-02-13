# AI4Med

| No. | Name | Paper Title | Pub |Imaging | Based | Main Contribution |  Abstract | Code |
|----:|--------|------------|------|------|------|-------------------|-----------|----------|
| 1   | [SLATER](https://arxiv.org/pdf/2105.08059) | Unsupervised MRI Reconstruction via Zero-Shot Learned Adversarial Transformers | TMI(2022) | MRI| Volume| Unsupervised MRI Reconstruction via Zero-Shot Learned Adversarial Transformers  | <details><summary>Click</summary> Supervised reconstruction models are characteristically trained on matched pairs of undersampled and fully-sampled data to capture an MRI prior, along with supervision regarding the imaging operator to enforce data consistency. To reduce supervision requirements, the recent deep image prior framework instead conjoins untrained MRI priors with the imaging operator during inference. Yet, canonical convolutional architectures are suboptimal in capturing long-range relationships, and priors based on randomly initialized networks may yield suboptimal performance. To address these limitations, here we introduce a novel unsupervised MRI reconstruction method based on zero-Shot Learned Adversarial TransformERs (SLATER). SLATER embodies a deep adversarial network with cross-attention transformers to map noise and latent variables onto coil-combined MR images. During pre-training, this unconditional network learns a high-quality MRI prior in an unsupervised generative modeling task. During inference, a zero-shot reconstruction is then performed by incorporating the imaging operator and optimizing the prior to maximize consistency to undersampled data. Comprehensive experiments on brain MRI datasets clearly demonstrate the superior performance of SLATER against state-of-the-art unsupervised methods. </details> | [🔗](https://github.com/icon-lab/SLATER)
| 2   | [DEER](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9239986) | Deep Efficient End-to-End Reconstruction
(DEER) Network for Few-View Breast CT Image Reconstruction | IEEE Access(2020) | CT | Volume | Deep efficient end-to-end reconstruction (DEER)network for few-view breast CT image reconstruction   | <details><summary>Click</summary> Breast CT provides image volumes with isotropic resolution in high contrast, enabling detection of small calcification (down to a few hundred microns in size) and subtle density differences. Since breast is sensitive to x-ray radiation, dose reduction of breast CT is an important topic, and for this purpose, few-view scanning is a main approach. In this article, we propose a Deep Efficient End-to-end Reconstruction (DEER) network for few-view breast CT image reconstruction. The major merits of our network include high dose efficiency, excellent image quality, and low model complexity. By the design, the proposed network can learn the reconstruction process with as few as (9(N) parameters, where N is the side length of an image to be reconstructed, which represents orders of magnitude improvements relative to the state-of-the-art deeplearning-based reconstruction methods that map raw data to tomographic images directly. Also, validated on a cone-beam breast CT dataset prepared by Koning Corporation on a commercial scanner, our method demonstrates a competitive performance over the state-of-the-art reconstruction networks in terms of image quality. The source code of this paper is available at: https://github.com/HuidongXie/DEER. </details> | [🔗](https://github.com/HuidongXie/DEER)

