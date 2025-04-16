# AI4Radiology

This project is created by ***Yuezhe Yang*** for paper "**Explicit and Implicit Representations in AI-based 3D Reconstruction for Radiology: A systematic literature review**" ([Paper Link](https://arxiv.org/pdf/2504.11349)). 

### [Project Page](https://.github.io)

## ***Abstract***

The demand for high-quality medical imaging in clinical practice and assisted diagnosis has made 3D reconstruction in radiological imaging a key research focus. Artificial intelligence (AI) has emerged as a promising approach to enhancing reconstruction accuracy while reducing acquisition and processing time, thereby minimizing patient radiation exposure and discomfort and ultimately benefiting clinical diagnosis. This review explores state-of-the-art AI-based 3D reconstruction algorithms in radiological imaging, categorizing them into explicit and implicit approaches based on their underlying principles. Explicit methods include point-based, volume-based, and Gaussian representations, while implicit methods encompass implicit prior embedding and neural radiance fields. Additionally, we examine commonly used evaluation metrics and benchmark datasets. Finally, we discuss the current state of development, key challenges, and future research directions in this evolving field. Our project available on: [this https URL](https://github.com/Bean-Young/AI4Med).

## ***Dataset***

In the task of 3D reconstruction in radiological imaging, publicly available datasets play a crucial role. High-quality, standardized data is essential for algorithm training, validation, and testing. Public datasets provide researchers with a unified benchmark, enabling fair comparisons of different methods under the same conditions, thereby facilitating algorithm optimization and advancement.

Unlike other medical imaging tasks, reconstruction often requires subjects to undergo two scans under comparable conditions, particularly maintaining consistent positioning, posture, and physiological state, in order to obtain corresponding test samples and ground truth data. Additionally, medical data is subject to strict legal and regulatory constraints due to patient privacy concerns, making data collection both challenging and costly. The availability of public datasets significantly lowers the barrier to data access. Our review provides the most comprehensive publicly available datasets for 3D reconstruction in radiological imaging tasks, including CT, MRI, PET, US, and Multi-modality datasets. The specific details are presented in Table below.

| No. | Name |Imaging |   Detail| Link |
|----:|--------|------|---------------------------------|-----------|
| 1 | VerSE | CT |A multi-center, multi-detector CT spine dataset for vertebral annotation and segmentation.| [🔗](https://paperswithcode.com/dataset/verse-1) |
|2 | LIDC-IDRI | CT |  A low-dose lung CT dataset for lung nodule classification, segmentation, and detection. | [🔗](https://paperswithcode.com/dataset/lidc-idri) |
|3 | COVID-CT-Dataset | CT | Contains COVID-19 CT images from patients and non-COVID-19 CTs | [🔗](https://paperswithcode.com/dataset/covid-ct) |
|4|Richard et al|CT|volumetric reconstructions of the chest cavity at 10 breathing phases |[🔗]( http://www.dir-lab.com) |
|5 | KiTS19 | CT | dataset of segmented CT imaging and treatment outcomes for 300 patients treated with partial or radical nephrectomy| [🔗](https://paperswithcode.com/dataset/kits19) |
|6 |LDCT | CT |contrast-enhanced abdominal CT patient scans, each acquired in the portal venous phase using a Siemens SOMATOM Flash scanner.  | [🔗](https://doi.org/10.7937/9npb-2637) |
|7 | CTSpine1K| CT|  Dataset curated from mutiple sources for spinal vertebrae segmentation and 3D spine reconstruction | [🔗](https://paperswithcode.com/dataset/ctspine1k) |
|8|MIDRC-RICORD-1B|CT|De-identified dataset from  COVID negative patients|[🔗](https://www.cancerimagingarchive.net/collection/midrc-ricord-1b/) |
|9|Corona-Figueroa et al.|CT|Digital Reconstructed Radiographs (DRRs) from chest and knee CT scans.|[🔗](https://github.com/abrilcf/mednerf) |
|10 |BraTS| MRI|Brain MRI scans from patients with gliomas, including four modalities: T1-weighted (T1), contrast-enhanced T1-weighted (T1Gd), T2-weighted (T2), and T2-FLAIR |[🔗](http://braintumorsegmentation.org/)|
|11  |IXI|MRI|T1, T2 and PD-weighted images, Diffusion-weighted and MRA images from normal, healthy subjects.|[🔗](https://brain-development.org/ixi-dataset/)|
|12   |ADNI| MRI|A collection of longitudinal clinical, imaging, genetic, and other biomarker data.|[🔗](https://adni.loni.usc.edu/data-samples/adni-data/)|
|13   |OASIS-1| MRI|Cross-sectional MRI Data in Young, Middle Aged, Nondemented, and Demented Older Adults|[🔗](https://sites.wustl.edu/oasisbrains/home/oasis-1/)|
|14  | FastMRI| MRI|k-space and image data of knee examinations for accelerated MR image reconstruction using machine learning|[🔗]( https://fastmri.med.nyu.edu/)|
|15   |HCP| MRI|High-level extensively processed data ; Group ICA-based parcellation + timeseries + netmats datasets.|[🔗](https://www.humanconnectome.org/study/hcp-young-adult/data-releases)|
|16 |Landman et al|MRI|Multimodal MRI dataset.|[🔗](http://www.nitrc.org/projects/multimodal/) | 
|17|FeTA|MRI|T2-weighted fetal brain reconstructions of both normal and pathological brains across various gestational ages. |[🔗](https://www.synapse.org/Synapse:syn25649159/wiki/610007) |
|18| Xu et al|MRI|volumetric MRI time series at a gestational age ranging from 25 to 35 weeks.|[🔗](https://link.springer.com/chapter/10.1007/978-3-030-87234-2_19) |
|19| dHCP| MRI|Anatomical, diffusion, and functional metadata, including brain segmentation and cortical surface.|[🔗](https://paperswithcode.com/dataset/dhcp)|
|20   |MSD| MRI|multiparametric magnetic resonance imaging (MRI) scans from patients diagnosed with either glioblastoma or lower-grade glioma|[🔗](http://medicaldecathlon.com/)|
|21   |DCE-MRI| MRI|DCE-MR images for benign and malignant breast tumor cases.|[🔗](https://github.com/smallboy-code/Breast-cancer-dataset?tab=readme-ov-file)|
| 22 |  OCMR|MRI|Multi-coil k-space data and undersampled cardiac cine series.  |[🔗](https://github.com/MRIOSU/OCMR)
|23   |SKMTEA| MRI|A dataset that pairs raw quantitative knee MRI (qMRI) data, image data, and dense annotations of tissue and pathology for end-to-end exploration and evaluation of the MR imaging pipeline.|[🔗](https://aimi.stanford.edu/datasets/skm-tea-knee-mri)|
|24|Aubert-Broche et al.|MRI|T1, T2, and proton density (PD)-weighted magnetic resonance imaging (MRI) scans from each subject.|[🔗](https://ieeexplore.ieee.org/abstract/document/1717639?signout=success) |
|25|CMRxRecon2024|MRI|Dataset include multi-contrast k-space data, consist of cardiac cine, T1/T2mapping, tagging, phase-contrast (i.e., flow2d), and dark-blood imaging. It also includes imaging of different anatomical views like long-axis (2-chamber, 3-chamber, and 4-chamber), short-axis (SAX), left ventricul outflow tract (LVOT), and aorta (transversal and sagittal views). |[🔗](https://www.synapse.org/#!Synapse:syn57407073/datasets/)|
|26|UDPET|PET|The dataset contains whole-body 18F-FDG PET imaging |[🔗](https://udpet-challenge.github.io/)|
|27 |Wysocki et al.| US|A dataset of synthetic liver ultrasound images and tracked spine phantom scans.|[🔗](https://github.com/magdalena-wysocki/ultra-nerf)|
|28 |MITEA| US|The largest publicly available 3DE dataset to date|[🔗](https://www.cardiacatlas.org/mitea/)|
|29| Papageorghiou et al.|US|A set of international standards for fetal growth to enhance the accuracy of diagnosing fetal growth restriction and improve clinical management|[🔗](https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(14)61490-2/fulltext?mod=article_inline)|
|30  |MMWHS| CT MRI|Three-dimensional CT and MRI images covering the entire heart for cardiac segmentation.|[🔗](https://www.kaggle.com/datasets/panhuiyang/mmwhs-datasets)|
|31  |OASIS-3| MRI PET|neuroimaging and processed imaging data in participants with normal aging and Alzheimer's Disease|[🔗](https://sites.wustl.edu/oasisbrains/home/oasis-3/)|
|32 | μ-RegPro |MR US|Dataset for assisting prostate biopsy and focal therapy, surgical and interventional tasks |[🔗](https://muregpro.github.io/data.html)

## ***Literature***

Explicit representations were initially used for AI-assisted reconstruction of radiological imaging. At first, the most typical explicit reconstruction methods were slice-based, meaning that experiments were conducted using individual slices. However, such methods overlooked the longitudinal continuity of radiology images, leading to severe artifacts or inconsistencies across slices. Later, volume-based reconstruction methods emerged. Unlike slice-based approaches, volume representations incorporate spatial information at each location, enabling more accurate restoration of radiology images. Recently, an explicit Gaussian representation integrated with neural radiance field concepts, known as 3DGS, has gained significant attention in radiological imaging due to its precise representation and high reconstruction efficiency. 

Unlike discrete explicit representations that directly encode features or signal values, implicit representations are defined as continuous generative functions that map input coordinates to corresponding values within the input space. Existing implicit representations in radiology imaging applications can be categorized into two main types: Implicit Prior Embedding (IPE) and Neural Radiance Fields (NRF). IPE incorporates prior information into the representation space or model parameter space, allowing the model to automatically learn features that conform to the given prior during training. On the other hand, NRF have gained attention in radiology imaging reconstruction since their introduction due to their ability to generate high-resolution, photorealistic images and render realistic 3D views from arbitrary perspectives.

The literature review can be found in Table below.

---
### Paper 01: [X2CT-GAN](https://openaccess.thecvf.com/content_CVPR_2019/papers/Ying_X2CT-GAN_Reconstructing_CT_From_Biplanar_X-Rays_With_Generative_Adversarial_Networks_CVPR_2019_paper.pdf)
- **Title**: X2CT-GAN: Reconstructing CT From Biplanar X-Rays With Generative Adversarial Networks  
- **Conference**: CVPR(2019)  
- **Imaging**: CT  
- **Based on**: Slice  
- **Main Contribution**:  
  A GAN-based model that reconstructs high-resolution 3D CT images from biplanar 2D X-rays using a specially designed generator and combined loss functions.  
- **Abstract**:  
  <details><summary>Click</summary>Computed tomography (CT) can provide a 3D view of the patient's internal organs, facilitating disease diagnosis, but it incurs more radiation dose to a patient and a CT scanner is much more cost prohibitive than an X-ray machine too. Traditional CT reconstruction methods require hundreds of X-ray projections through a full rotational scan of the body, which cannot be performed on a typical X-ray machine. In this work, we propose to reconstruct CT from two orthogonal X-rays using the generative adversarial network (GAN) framework. A specially designed generator network is exploited to increase data dimension from 2D (X-rays) to 3D (CT), which is not addressed in previous research of GAN. A novel feature fusion method is proposed to combine information from two X-rays. The mean squared error (MSE) loss and adversarial loss are combined to train the generator, resulting in a high-quality CT volume both visually and quantitatively. Extensive experiments on a publicly available chest CT dataset demonstrate the effectiveness of the proposed method. It could be a nice enhancement of a low-cost X-ray machine to provide physicians a CT-like 3D volume in several niche applications.</details>  
- **Code**: ❌

---
### Paper 02: [CTTR](https://www.sciencedirect.com/science/article/pii/S1120179722020154?casa_token=Mdbm9fp-4jUAAAAA:ii0SPXB6Gu78vHYhCDRpD_EnF1EgPgKwJkIuTFQt4bn3XafYjbAqZAPbTAx8X7zXPCQte1bo4LFw)
- **Title**: Dual-domain sparse-view CT reconstruction with Transformers  
- **Conference**: Physica Medica(2022)  
- **Imaging**: CT  
- **Based on**: Slice  
- **Main Contribution**:  
  Introduce a highly efficient deep learning model for few-view breast CT reconstruction, achieving high image quality with low model complexity.  
- **Abstract**:  
  <details><summary>Click</summary>Purpose:Computed Tomography (CT) has been widely used in the medical field. Sparse-view CT is an effective and feasible method to reduce the radiation dose. However, the conventional filtered back projection (FBP) algorithm will suffer from severe artifacts in sparse-view CT. Iterative reconstruction algorithms have been adopted to remove artifacts, but they are time-consuming due to repeated projection and back projection and may cause blocky effects. To overcome the difficulty in sparse-view CT, we proposed a dual-domain sparse-view CT algorithm CT Transformer (CTTR) and paid attention to sinogram information.Methods:CTTR treats sinograms as sentences and enhances reconstructed images with sinogram’s characteristics. We qualitatively evaluate the CTTR, an iterative method TVM-POCS, a convolutional neural network based method FBPConvNet in terms of a reduction in artifacts and a preservation of details. Besides, we also quantitatively evaluate these methods in terms of RMSE, PSNR and SSIM.Results:We evaluate our method on the Lung Image Database Consortium image collection with different numbers of projection views and noise levels. Experiment studies show that, compared with other methods, CTTR can reduce more artifacts and preserve more details on various scenarios. Specifically, CTTR improves the FBPConvNet performance of PSNR by 0.76 dB with 30 projections.Conclusions:The performance of our proposed CTTR is better than the method based on CNN in the case of extremely sparse views both on visual results and quantitative evaluation. Our proposed method provides a new idea for the application of Transformers to CT image processing.</details>  
- **Code**: ❌

---
### Paper 03: [DuDoTrans](https://link.springer.com/chapter/10.1007/978-3-031-17247-2_9)
- **Title**: DuDoTrans: Dual-Domain Transformer for Sparse-View CT Reconstruction  
- **Conference**: MLMIR(2022)  
- **Imaging**: CT  
- **Based on**: Slice  
- **Main Contribution**:  
  Utilize the long-range dependency modeling capability of the Transformer to restore informative sinograms, and subsequently reconstruct the CT image using both the enhanced sinograms and the original sinograms.  
- **Abstract**:  
  <details><summary>Click</summary>While Computed Tomography (CT) is necessary for clinical diagnosis, ionizing radiation in the imaging process induces irreversible injury, thereby driving researchers to study sparse-view CT reconstruction. Iterative models are proposed to alleviate the appeared artifacts in sparse-view CT images, but their computational cost is expensive. Deep-learning-based methods have gained prevalence due to the excellent reconstruction performances and computation efficiency. However, these methods ignore the mismatch between the CNN’s local feature extraction capability and the sinogram’s global characteristics. To overcome the problem, we propose Dual-Domain Transformer (DuDoTrans) to simultaneously restore informative sinograms via the long-range dependency modeling capability of Transformer and reconstruct CT image with both the enhanced and raw sinograms. With such a novel design, DuDoTrans even with fewer involved parameters is more effective and generalizes better than competing methods, which is confirmed by reconstruction performances on the NIH-AAPM and COVID-19 datasets. Finally, experiments also demonstrate its robustness to noise.</details>  
- **Code**: ❌

---
### Paper 04: [CoreDiff](https://arxiv.org/pdf/2304.01814)
- **Title**: CoreDiff: Contextual Error-Modulated Generalized Diffusion Model for Low-Dose CT Denoising and Generalization  
- **Conference**: IEEE TMI(2023)  
- **Imaging**: CT  
- **Based on**: Slice  
- **Main Contribution**:  
  A diffusion-based model using a mean-preserving degradation operator and CLEAR-Net for low-dose CT denoising, enhancing image quality with fewer sampling steps.  
- **Abstract**:  
  <details><summary>Click</summary>Low-dose computed tomography (CT) images suffer from noise and artifacts due to photon starvation and electronic noise. Recently, some works have attempted to use diffusion models to address the over-smoothness and training instability encountered by previous deep-learning-based denoising models. However, diffusion models suffer from long inference time due to a large number of sampling steps involved. Very recently, cold diffusion model generalizes classical diffusion models and has greater flexibility. Inspired by cold diffusion, this paper presents a novel COntextual eRror-modulated gEneralized Diffusion model for low-dose CT (LDCT) denoising, termed CoreDiff. First, CoreDiff utilizes LDCT images to displace the random Gaussian noise and employs a novel mean-preserving degradation operator to mimic the physical process of CT degradation, significantly reducing sampling steps thanks to the informative LDCT images as the starting point of the sampling process. Second, to alleviate the error accumulation problem caused by the imperfect restoration operator in the sampling process, we propose a novel ContextuaL Error-modulAted Restoration Network (CLEAR-Net), which can leverage contextual information to constrain the sampling process from structural distortion and modulate time step embedding features for better alignment with the input at the next time step. Third, to rapidly generalize the trained model to a new, unseen dose level with as few resources as possible, we devise a one-shot learning framework to make CoreDiff generalize faster and better using only one single LDCT image (un)paired with normal-dose CT (NDCT). Extensive experimental results on four datasets demonstrate that our CoreDiff outperforms competing methods in denoising and generalization performance, with clinically acceptable inference time. Source code is made available at https://github.com/qgao21/CoreDiff.</details>  
- **Code**: [🔗](https://github.com/qgao21/CoreDiff)

---
### Paper 05: [Du et al.](https://www.sciencedirect.com/science/article/pii/S0925231219304771)
- **Title**: Super-resolution reconstruction of single anisotropic 3D MR images using residual convolutional neural network  
- **Conference**: Neucom.(2020)  
- **Imaging**: MRI  
- **Based on**: Slice  
- **Main Contribution**:  
  A deep learning model using residual learning and skip connections for super-resolution reconstruction of 3D MRI images.  
- **Abstract**:  
  <details><summary>Click</summary> High-resolution (HR) magnetic resonance (MR) imaging is an important diagnostic technique in clinical practice. However, hardware limitations and time constraints often result in the acquisition of anisotropic MR images. It is highly desirable but very challenging to enhance image spatial resolution in medical image analysis for disease diagnosis. Recently, studies have shown that deep convolutional neural networks (CNN) can significantly boost the performance of MR image super-resolution (SR) reconstruction. In this paper, we present a novel CNN-based anisotropic MR image reconstruction method based on residual learning with long and short skip connections. The proposed network can effectively alleviate the vanishing gradient problem of deep networks and learn to restore high-frequency details of MR images. To reduce computational complexity and memory usage, the proposed network utilizes cross-plane self-similarity of 3D T1-weighted (T1w) MR images. Based on experiments on simulated and clinical brain MR images, we demonstrate that the proposed network can significantly improve the spatial resolution of anisotropic MR images with high computational efficiency. The network trained on T1w MR images is able to effectively reconstruct both SR T1w and T2-weighted (T2w) images, exploiting image features for multi-modality reconstruction. Moreover, the experimental results show that the proposed method outperforms classical interpolation methods, non-local means method (NLM), and sparse coding based algorithm in terms of peak signal-to-noise-ratio, structural similarity image index, intensity profile, and small structures. The proposed method can be efficiently applied to SR reconstruction of thick-slice MR images in the out-of-plane views for radiological assessment and post-acquisition processing.</details>  
- **Code**: ❌

---
### Paper 06: [SLATER](https://arxiv.org/pdf/2105.08059)
- **Title**: Unsupervised MRI Reconstruction via Zero-Shot Learned Adversarial Transformers  
- **Conference**: TMI(2022)  
- **Imaging**: MRI  
- **Based on**: Slice  
- **Main Contribution**:  
  Introduce an unsupervised MRI reconstruction method using adversarial transformers to learn MRI priors and perform zero-shot inference for improved image quality.  
- **Abstract**:  
  <details><summary>Click</summary> Supervised reconstruction models are characteristically trained on matched pairs of undersampled and fully-sampled data to capture an MRI prior, along with supervision regarding the imaging operator to enforce data consistency. To reduce supervision requirements, the recent deep image prior framework instead conjoins untrained MRI priors with the imaging operator during inference. Yet, canonical convolutional architectures are suboptimal in capturing long-range relationships, and priors based on randomly initialized networks may yield suboptimal performance. To address these limitations, here we introduce a novel unsupervised MRI reconstruction method based on zero-Shot Learned Adversarial TransformERs (SLATER). SLATER embodies a deep adversarial network with cross-attention transformers to map noise and latent variables onto coil-combined MR images. During pre-training, this unconditional network learns a high-quality MRI prior in an unsupervised generative modeling task. During inference, a zero-shot reconstruction is then performed by incorporating the imaging operator and optimizing the prior to maximize consistency to undersampled data. Comprehensive experiments on brain MRI datasets clearly demonstrate the superior performance of SLATER against state-of-the-art unsupervised methods. </details>  
- **Code**: [🔗](https://github.com/icon-lab/SLATER)

---
### Paper 07: [PCNN](https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/abs/10.1002/nbm.4405)
- **Title**: Rapid reconstruction of highly undersampled, non-Cartesian real-time cine k-space data using a perceptual complex neural network (PCNN)  
- **Conference**: NMRB(2021)  
- **Imaging**: MRI  
- **Based on**: Slice  
- **Main Contribution**:  
  A perceptual complex neural network for rapid reconstruction of undersampled MRI data using complex convolution and perceptual loss.  
- **Abstract**:  
  <details><summary>Click</summary>Highly accelerated real-time cine MRI using compressed sensing (CS) is a promising approach to achieve high spatio-temporal resolution and clinically acceptable image quality in patients with arrhythmia and/or dyspnea. However, its lengthy image reconstruction time may hinder its clinical translation. The purpose of this study was to develop a neural network for reconstruction of non-Cartesian real-time cine MRI k-space data faster (<1 min per slice with 80 frames) than graphics processing unit (GPU)-accelerated CS reconstruction, without significant loss in image quality or accuracy in left ventricular (LV) functional parameters. We introduce a perceptual complex neural network (PCNN) that trains on complex-valued MRI signal and incorporates a perceptual loss term to suppress incoherent image details. This PCNN was trained and tested with multi-slice, multi-phase, cine images from 40 patients (20 for training, 20 for testing), where the zero-filled images were used as input and the corresponding CS reconstructed images were used as practical ground truth. The resulting images were compared using quantitative metrics (structural similarity index (SSIM) and normalized root mean square error (NRMSE)) and visual scores (conspicuity, temporal fidelity, artifacts, and noise scores), individually graded on a five-point scale (1, worst; 3, acceptable; 5, best), and LV ejection fraction (LVEF). The mean processing time per slice with 80 frames for PCNN was 23.7 ± 1.9 s for pre-processing (Step 1, same as CS) and 0.822 ± 0.004 s for dealiasing (Step 2, 166 times faster than CS). Our PCNN produced higher data fidelity metrics (SSIM = 0.88 ± 0.02, NRMSE = 0.014 ± 0.004) compared with CS. While all the visual scores were significantly different (P < 0.05), the median scores were all 4.0 or higher for both CS and PCNN. LVEFs measured from CS and PCNN were strongly correlated (R2 = 0.92) and in good agreement (mean difference = −1.4% [2.3% of mean]; limit of agreement = 10.6% [17.6% of mean]). The proposed PCNN is capable of rapid reconstruction (25 s per slice with 80 frames) of non-Cartesian real-time cine MRI k-space data, without significant loss in image quality or accuracy in LV functional parameters.</details>  
- **Code**: ❌

---
### Paper 08: [Wei et al.](https://aapm.onlinelibrary.wiley.com/doi/abs/10.1002/mp.16141)
- **Title**: Real-time 3D MRI reconstruction from cine-MRI using unsupervised network in MRI-guided radiotherapy for liver cancer  
- **Conference**: Med. Phys.(2022)  
- **Imaging**: MRI  
- **Based on**: Slice  
- **Main Contribution**:  
  An unsupervised deep learning model for real-time 3D MRI reconstruction from cine-MRI, using deformation vector fields to estimate respiratory motion.  
- **Abstract**:  
  <details><summary>Click</summary>Purpose Respiration has a major impact on the accuracy of radiation treatment for thorax and abdominal tumours. Instantaneous volumetric imaging could provide precise knowledge of tumour and normal organs’ three-dimensional (3D) movement, which is the key to reducing the negative effect of breathing motion. Therefore, this study proposed a real-time 3D MRI reconstruction method from cine-MRI using an unsupervised network.Methods and materials Cine-MRI and setup 3D-MRI from eight patients with liver cancer were utilized to establish and validate the deep learning network for 3D-MRI reconstruction. Unlike previous methods that required 4D-MRI for network training, the proposed method utilized a reference 3D-MRI and cine-MRI to generate the training data. Then, a network was trained in an unsupervised manner to estimate the relationship between the cine-MRI acquired on coronal plane and deformation vector field (DVF) that describes the patient's breathing motion. After the training process, the coronal cine-MRI were inputted into the network, and the corresponding DVF was obtained. By wrapping the reference 3D-MRI with the generated DVF, the 3D-MRI could be reconstructed.Results The reconstructed 3D-MRI slices were compared with the corresponding phase-sorted cine-MRI using dice similarity coefficients (DSCs) of liver contours and blood vessel localization error. In all patients, the liver DSC had mean value >96.1% and standard deviation < 1.3%; the blood vessel localization error had mean value <2.6 mm, and standard deviation was <2.0 mm. Moreover, the time for 3D-MRI reconstruction was approximately 100 ms. These results indicated that the proposed method could accurately reconstruct the 3D-MRI in real time.Conclusions The proposed method could accurately reconstruct the 3D-MRI from cine-MRI in real time. This method has great potential in improving the accuracy of radiotherapy for moving tumours.</details>  
- **Code**: ❌

---
### Paper 09: [MCAD](https://arxiv.org/pdf/2406.13150)
- **Title**: MCAD: Multi-modal Conditioned Adversarial Diffusion Model for High-Quality PET Image Reconstruction  
- **Conference**: MICCAI(2024)  
- **Imaging**: PET  
- **Based on**: Slice  
- **Main Contribution**:  
  A multi-modal conditioned adversarial diffusion model for reconstructing high-quality PET images from low-dose PET and clinical data using diffusion processes and semantic consistency.  
- **Abstract**:  
  <details><summary>Click</summary>Radiation hazards associated with standard-dose positron emission tomography (SPET) images remain a concern, whereas the quality of low-dose PET (LPET) images fails to meet clinical requirements. Therefore, there is great interest in reconstructing SPET images from LPET images. However, prior studies focus solely on image data, neglecting vital complementary information from other modalities, e.g., patients’ clinical tabular, resulting in compromised reconstruction with limited diagnostic utility. Moreover, they often overlook the semantic consistency between real SPET and reconstructed images, leading to distorted semantic contexts. To tackle these problems, we propose a novel Multi-modal Conditioned Adversarial Diffusion model (MCAD) to reconstruct SPET images from multi-modal inputs, including LPET images and clinical tabular. Specifically, our MCAD incorporates a Multi-modal conditional Encoder (Mc-Encoder) to extract multi-modal features, followed by a conditional diffusion process to blend noise with multi-modal features and gradually map blended features to the target SPET images. To balance multi-modal inputs, the Mc-Encoder embeds Optimal Multi-modal Transport co-Attention (OMTA) to narrow the heterogeneity gap between image and tabular while capturing their interactions, providing sufficient guidance for reconstruction. In addition, to mitigate semantic distortions, we introduce the Multi-Modal Masked Text Reconstruction (M3TRec), which leverages semantic knowledge extracted from denoised PET images to restore the masked clinical tabular, thereby compelling the network to maintain accurate semantics during reconstruction. To expedite the diffusion process, we further introduce an adversarial diffusive network with a reduced number of diffusion steps. Experiments show that our method achieves the state-of-the-art performance both qualitatively and quantitatively.</details>  
- **Code**: ❌

---
### Paper 10: [MEaTransGAN](https://www.sciencedirect.com/science/article/abs/pii/S1361841523002438)
- **Title**: 3D multi-modality Transformer-GAN for high-quality PET reconstruction  
- **Conference**: MIA(2024)  
- **Imaging**: PET  
- **Based on**: Slice  
- **Main Contribution**:  
  A novel deep learning model that integrates CNNs, Transformer, and GANs to reconstruct high-quality standard-dose PET images from low-dose PET and T1-MRI images, enhancing diagnostic value while reducing radiation exposure.  
- **Abstract**:  
  <details><summary>Click</summary>Positron emission tomography (PET) scans can reveal abnormal metabolic activities of cells and provide favorable information for clinical patient diagnosis. Generally, standard-dose PET (SPET) images contain more diagnostic information than low-dose PET (LPET) images but higher-dose scans can also bring higher potential radiation risks. To reduce the radiation risk while acquiring high-quality PET images, in this paper, we propose a 3D multi-modality edge-aware Transformer-GAN for high-quality SPET reconstruction using the corresponding LPET images and T1 acquisitions from magnetic resonance imaging (T1-MRI). Specifically, to fully excavate the metabolic distributions in LPET and anatomical structural information in T1-MRI, we first use two separate CNN-based encoders to extract local spatial features from the two modalities, respectively, and design a multimodal feature integration module to effectively integrate the two kinds of features given the diverse contributions of features at different locations. Then, as CNNs can describe local spatial information well but have difficulty in modeling long-range dependencies in images, we further apply a Transformer-based encoder to extract global semantic information in the input images and use a CNN decoder to transform the encoded features into SPET images. Finally, a patch-based discriminator is applied to ensure the similarity of patch-wise data distribution between the reconstructed and real images. Considering the importance of edge information in anatomical structures for clinical disease diagnosis, besides voxel-level estimation error and adversarial loss, we also introduce an edge-aware loss to retain more edge detail information in the reconstructed SPET images. Experiments on the phantom dataset and clinical dataset validate that our proposed method can effectively reconstruct high-quality SPET images and outperform current state-of-the-art methods in terms of qualitative and quantitative metrics.</details>  
- **Code**: ❌

---
### Paper 11: [Singh et al.](https://arxiv.org/pdf/2308.14190)
- **Title**: Score-Based Generative Models for PET Image Reconstruction  
- **Conference**: MELBA(2024)  
- **Imaging**: PET  
- **Based on**: Slice  
- **Main Contribution**:  
  A 3D PET reconstruction framework using score-based generative models with a novel PET-DDS sampling method to improve image quality and robustness.  
- **Abstract**:  
  <details><summary>Click</summary>Score-based generative models have demonstrated highly promising results for medical image reconstruction tasks in magnetic resonance imaging or computed tomography. However, their application to Positron Emission Tomography (PET) is still largely unexplored. PET image reconstruction involves a variety of challenges, including Poisson noise with high variance and a wide dynamic range. To address these challenges, we propose several PET-specific adaptations of score-based generative models. The proposed framework is developed for both 2D and 3D PET. In addition, we provide an extension to guided reconstruction using magnetic resonance images. We validate the approach through extensive 2D and 3D in-silico experiments with a model trained on patient-realistic data without lesions, and evaluate on data without lesions as well as out-of-distribution data with lesions. This demonstrates the proposed method's robustness and significant potential for improved PET reconstruction.</details>  
- **Code**: ❌

---
### Paper 12: [MambaMIR](https://www.sciencedirect.com/science/article/pii/S1361841524002597)
- **Title**: Enhancing global sensitivity and uncertainty quantification in medical image reconstruction with Monte Carlo arbitrary-masked mamba  
- **Conference**: MIA(2025)  
- **Imaging**: CT MRI  
- **Based on**: Slice  
- **Main Contribution**:  
  Enhancing global sensitivity and uncertainty quantification in medical image reconstruction with Monte Carlo arbitrary-masked mamba.  
- **Abstract**:  
  <details><summary>Click</summary>Deep learning has been extensively applied in medical image reconstruction, where Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs) represent the predominant paradigms, each possessing distinct advantages and inherent limitations: CNNs exhibit linear complexity with local sensitivity, whereas ViTs demonstrate quadratic complexity with global sensitivity. The emerging Mamba has shown superiority in learning visual representation, which combines the advantages of linear scalability and global sensitivity. In this study, we introduce MambaMIR, an Arbitrary-Masked Mamba-based model with wavelet decomposition for joint medical image reconstruction and uncertainty estimation. A novel Arbitrary Scan Masking (ASM) mechanism “masks out” redundant information to introduce randomness for further uncertainty estimation. Compared to the commonly used Monte Carlo (MC) dropout, our proposed MC-ASM provides an uncertainty map without the need for hyperparameter tuning and mitigates the performance drop typically observed when applying dropout to low-level tasks. For further texture preservation and better perceptual quality, we employ the wavelet transformation into MambaMIR and explore its variant based on the Generative Adversarial Network, namely MambaMIR-GAN. Comprehensive experiments have been conducted for multiple representative medical image reconstruction tasks, demonstrating that the proposed MambaMIR and MambaMIR-GAN outperform other baseline and state-of-the-art methods in different reconstruction tasks, where MambaMIR achieves the best reconstruction fidelity and MambaMIR-GAN has the best perceptual quality. In addition, our MC-ASM provides uncertainty maps as an additional tool for clinicians, while mitigating the typical performance drop caused by the commonly used dropout.</details>  
- **Code**: ❌

---
### Paper 13: [Restore-RWKV](https://arxiv.org/pdf/2407.11087)
- **Title**: Restore-RWKV: Efficient and Effective Medical Image Restoration with RWKV  
- **Conference**: arxiv(2024)  
- **Imaging**: CT MRI PET  
- **Based on**: Slice  
- **Main Contribution**:  
  Restore-RWKV innovatively incorporates a recurrent WKV attention mechanism with linear computational complexity and an omnidirectional token shift mechanism.  
- **Abstract**:  
  <details><summary>Click</summary>Transformers have revolutionized medical image restoration, but the quadratic complexity still poses limitations for their application to high-resolution medical images. The recent advent of the Receptance Weighted Key Value (RWKV) model in the natural language processing field has attracted much attention due to its ability to process long sequences efficiently. To leverage its advanced design, we propose Restore-RWKV, the first RWKV-based model for medical image restoration. Since the original RWKV model is designed for 1D sequences, we make two necessary modifications for modeling spatial relations in 2D medical images. First, we present a recurrent WKV (Re-WKV) attention mechanism that captures global dependencies with linear computational complexity. Re-WKV incorporates bidirectional attention as basic for a global receptive field and recurrent attention to effectively model 2D dependencies from various scan directions. Second, we develop an omnidirectional token shift (Omni-Shift) layer that enhances local dependencies by shifting tokens from all directions and across a wide context range. These adaptations make the proposed Restore-RWKV an efficient and effective model for medical image restoration. Even a lightweight variant of Restore-RWKV, with only 1.16 million parameters, achieves comparable or even superior results compared to existing state-of-the-art (SOTA) methods. Extensive experiments demonstrate that the resulting Restore-RWKV achieves SOTA performance across a range of medical image restoration tasks, including PET image synthesis, CT image denoising, MRI image super-resolution, and all-in-one medical image restoration. Code is available at: this https URL.</details>  
- **Code**: [🔗](https://github.com/Yaziwel/Restore-RWKV.git)

---
### Paper 14: [DEER](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9239986)
- **Title**: Deep Efficient End-to-End Reconstruction(DEER) Network for Few-View Breast CT Image Reconstruction  
- **Conference**: Access(2020)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  Introduce a highly efficient deep learning model for few-view breast CT reconstruction, achieving high image quality with low model complexity.  
- **Abstract**:  
  <details><summary>Click</summary> Breast CT provides image volumes with isotropic resolution in high contrast, enabling detection of small calcification (down to a few hundred microns in size) and subtle density differences. Since breast is sensitive to x-ray radiation, dose reduction of breast CT is an important topic, and for this purpose, few-view scanning is a main approach. In this article, we propose a Deep Efficient End-to-end Reconstruction (DEER) network for few-view breast CT image reconstruction. The major merits of our network include high dose efficiency, excellent image quality, and low model complexity. By the design, the proposed network can learn the reconstruction process with as few as (9(N) parameters, where N is the side length of an image to be reconstructed, which represents orders of magnitude improvements relative to the state-of-the-art deeplearning-based reconstruction methods that map raw data to tomographic images directly. Also, validated on a cone-beam breast CT dataset prepared by Koning Corporation on a commercial scanner, our method demonstrates a competitive performance over the state-of-the-art reconstruction networks in terms of image quality. The source code of this paper is available at: https://github.com/HuidongXie/DEER. </details>  
- **Code**: [🔗](https://github.com/HuidongXie/DEER)

---
### Paper 15: [HDnet](https://ieeexplore.ieee.org/abstract/document/9153172)
- **Title**: Hybrid-domain neural network processing for sparse-view CT reconstruction  
- **Conference**: TRPMS(2020)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  A hybrid-domain neural network approach for SVCT reconstruction, suitable for cone-beam CT imaging with low memory demands.  
- **Abstract**:  
  <details><summary>Click</summary>X-ray computed tomography (CT) is one of the most widely used tools in medical imaging, industrial nondestructive testing, lesion detection, and other applications. However, decreasing the projection number to lower the X-ray radiation dose usually leads to severe streak artifacts. To improve the quality of the images reconstructed from sparse-view projection data, we developed a hybrid-domain neural network (HDNet) processing for sparse-view CT (SVCT) reconstruction in this study. The HDNet decomposes the SVCT reconstruction problem into two stages and each stage focuses on one mission, which reduces the learning difficulty of the entire network. Experiments based on the simulated and clinical datasets are performed to demonstrate the performance of the proposed method. Compared with other competitive algorithms, quantitative and qualitative results show that the proposed method makes a great improvement on artifact suppression, tiny structure restoration, and contrast retention.</details>  
- **Code**: ❌

---
### Paper 16: [Singh et al.](https://ajronline.org/doi/pdf/10.2214/AJR.19.21809)
- **Title**: Image Quality and Lesion  Detection on Deep Learning  Reconstruction and Iterative  Reconstruction of Submillisievert  Chest and Abdominal CT  
- **Conference**: AJR(2020)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  DLR outperforms commercial IR and FBP in image quality and lesion detection when used at submillisievert doses for chest and abdominopelvic CT.  
- **Abstract**:  
  <details><summary>Click</summary>OBJECTIVE. The objective of this study was to compare image quality and clinically significant lesion detection on deep learning reconstruction (DLR) and iterative reconstruction (IR) images of submillisievert chest and abdominopelvic CT. MATERIALS AND METHODS. Our prospective multiinstitutional study included 59 adult patients (33 women, 26 men; mean age ± SD, 65 ± 12 years old; mean body mass index [weight in kilograms divided by the square of height in meters] = 27 ± 5) who underwent routine chest (n = 22; 16 women, six men) and abdominopelvic (n = 37; 17 women, 20 men) CT on a 640-MDCT scanner (Aquilion ONE, Canon Medical Systems). All patients gave written informed consent for the acquisition of low-dose (LD) CT (LDCT) after a clinically indicated standard-dose (SD) CT (SDCT). The SDCT series (120 kVp, 164–644 mA) were reconstructed with interactive reconstruction (IR) (adaptive iterative dose reduction [AIDR] 3D, Canon Medical Systems), and the LDCT (100 kVp, 120 kVp; 30–50 mA) were reconstructed with filtered back-projection (FBP), IR (AIDR 3D and forward-projected model-based iterative reconstruction solution [FIRST], Canon Medical Systems), and deep learning reconstruction (DLR) (Advanced Intelligent Clear-IQ Engine [AiCE], Canon Medical Systems). Four subspecialty-trained radiologists first read all LD image sets and then compared them side-by-side with SD AIDR 3D images in an independent, randomized, and blinded fashion. Subspecialty radiologists assessed image quality of LDCT images on a 3-point scale (1 = unacceptable, 2 = suboptimal, 3 = optimal). Descriptive statistics were obtained, and the Wilcoxon sign rank test was performed. RESULTS. Mean volume CT dose index and dose-length product for LDCT (2.1 ± 0.8 mGy, 49 ± 13mGy·cm) were lower than those for SDCT (13 ± 4.4 mGy, 567 ± 249 mGy·cm) (p < 0.0001). All 31 clinically significant abdominal lesions were seen on SD AIDR 3D and LD DLR images. Twenty-five, 18, and seven lesions were detected on LD AIDR 3D, LD FIRST, and LD FBP images, respectively. All 39 pulmonary nodules detected on SD AIDR 3D images were also noted on LD DLR images. LD DLR images were deemed acceptable for interpretation in 97% (35/37) of abdominal and 95–100% (21–22/22) of chest LDCT studies (p = 0.2–0.99). The LD FIRST, LD AIDR 3D, and LD FBP images had inferior image quality compared with SD AIDR 3D images (p < 0.0001). CONCLUSION. At submillisievert chest and abdominopelvic CT doses, DLR enables image quality and lesion detection superior to commercial IR and FBP images.</details>  
- **Code**: ❌

---
### Paper 17: [DLR](https://pubs.rsna.org/doi/pdf/10.1148/radiol.2020202317)
- **Title**: Improving Image Quality and Reducing Radiation Dose for Pediatric CT by Using Deep Learning Reconstruction  
- **Conference**: Radiol.(2020)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  While maintaining noise texture and spatial resolution, DLR significantly enhances image quality and reduces radiation dose in pediatric CT examinations.  
- **Abstract**:  
  <details><summary>Click</summary>Background CT deep learning reconstruction (DLR) algorithms have been developed to remove image noise. How the DLR affects image quality and radiation dose reduction has yet to be fully investigated. Purpose To investigate a DLR algorithm’s dose reduction and image quality improvement for pediatric CT. Materials and Methods DLR was compared with filtered back projection (FBP), statistical-based iterative reconstruction (SBIR), and model-based iterative reconstruction (MBIR) in a retrospective study by using data from CT examinations of pediatric patients (February to December 2018). A comparison of object detectability for 15 objects (diameter, 0.5–10 mm) at four contrast difference levels (50, 150, 250, and 350 HU) was performed by using a non-prewhitening-matched mathematical observer model with eye filter (d’NPWE), task transfer function, and noise power spectrum analysis. Object detectability was assessed by using area under the curve analysis. Three pediatric radiologists performed an observer study to assess anatomic structures with low object-to-background signal and contrast to noise in the azygos vein, right hepatic vein, common bile duct, and superior mesenteric artery. Observers rated from 1 to 10 (worst to best) for edge definition, quantum noise level, and object conspicuity. Analysis of variance and Tukey honest significant difference post hoc tests were used to analyze differences between reconstruction algorithms. Results Images from 19 patients (mean age, 11 years ± 5 [standard deviation]; 10 female patients) were evaluated. Compared with FBP, SBIR, and MBIR, DLR demonstrated improved object detectability by 51% (16.5 of 10.9), 18% (16.5 of 13.9), and 11% (16.5 of 14.8), respectively. DLR reduced image noise without noise texture effects seen with MBIR. Radiologist ratings were 7 ± 1 (DLR), 6.2 ± 1 (MBIR), 6.2 ± 1 (SBIR), and 4.6 ± 1 (FBP); two-way analysis of variance showed a difference on the basis of reconstruction type (P < .001). Radiologists consistently preferred DLR images (intraclass correlation coefficient, 0.89; 95% CI: 0.83, 0.93). DLR demonstrated 52% (1 of 2.1) greater dose reduction than SBIR. Conclusion The DLR algorithm improved image quality and dose reduction without sacrificing noise texture and spatial resolution.</details>  
- **Code**: ❌

---
### Paper 18: [DIOR](https://ieeexplore.ieee.org/abstract/document/9698177)
- **Title**: DIOR: Deep Iterative Optimization-Based Residual-Learning for Limited-Angle CT Reconstruction  
- **Conference**: TMI(2022)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  DIOR integrates iterative optimization and deep residual learning to enhance limited-angle CT reconstruction, improving artifact removal and detail preservation.  
- **Abstract**:  
  <details><summary>Click</summary>Limited-angle CT is a challenging problem in real applications. Incomplete projection data will lead to severe artifacts and distortions in reconstruction images. To tackle this problem, we propose a novel reconstruction framework termed Deep Iterative Optimization-based Residual-learning (DIOR) for limited-angle CT. Instead of directly deploying the regularization term on image space, the DIOR combines iterative optimization and deep learning based on the residual domain, significantly improving the convergence property and generalization ability. Specifically, the asymmetric convolutional modules are adopted to strengthen the feature extraction capacity in smooth regions for deep priors. Besides, in our DIOR method, the information contained in low-frequency and high-frequency components is also evaluated by perceptual loss to improve the performance in tissue preservation. Both simulated and clinical datasets are performed to validate the performance of DIOR. Compared with existing competitive algorithms, quantitative and qualitative results show that the proposed method brings a promising improvement in artifact removal, detail restoration and edge preservation.</details>  
- **Code**: ❌

---
### Paper 19: [FreeSeed](https://arxiv.org/pdf/2307.05890)
- **Title**: FreeSeed: Frequency-Band-Aware and Self-guided Network for Sparse-View CT Reconstruction  
- **Conference**: MICCAI(2023)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  Propose a frequency-band-aware and self-guided network to effectively remove artifacts and restore details in sparse-view CT images.  
- **Abstract**:  
  <details><summary>Click</summary>Sparse-view computed tomography (CT) is a promising solution for expediting the scanning process and mitigating radiation exposure to patients, the reconstructed images, however, contain severe streak artifacts, compromising subsequent screening and diagnosis. Recently, deep learning-based image post-processing methods along with their dual-domain counterparts have shown promising results. However, existing methods usually produce over-smoothed images with loss of details due to i) the difficulty in accurately modeling the artifact patterns in the image domain, and ii) the equal treatment of each pixel in the loss function. To address these issues, we concentrate on the image post-processing and propose a simple yet effective FREquency-band-awarE and SElf-guidED network, termed FreeSeed, which can effectively remove artifacts and recover missing details from the contaminated sparse-view CT images. Specifically, we first propose a frequency-band-aware artifact modeling network (FreeNet), which learns artifact-related frequency-band attention in the Fourier domain for better modeling the globally distributed streak artifact on the sparse-view CT images. We then introduce a self-guided artifact refinement network (SeedNet), which leverages the predicted artifact to assist FreeNet in continuing to refine the severely corrupted details. Extensive experiments demonstrate the superior performance of FreeSeed and its dual-domain counterpart over the state-of-the-art sparse-view CT reconstruction methods. Source code is made available at https://github.com/Masaaki-75/freeseed.</details>  
- **Code**: [🔗](https://github.com/Masaaki-75/freeseed)

---
### Paper 20: [DiffusionMBIR](https://openaccess.thecvf.com/content/CVPR2023/papers/Chung_Solving_3D_Inverse_Problems_Using_Pre-Trained_2D_Diffusion_Models_CVPR_2023_paper.pdf)
- **Title**: Solving 3D Inverse Problems Using Pre-Trained 2D Diffusion Models  
- **Conference**: CVRP(2023)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  Combine the ideas from the conventional model-based iterative reconstruction with the modern diffusion models.  
- **Abstract**:  
  <details><summary>Click</summary>Diffusion models have emerged as the new state-of-the-art generative model with high quality samples, with intriguing properties such as mode coverage and high flexibility. They have also been shown to be effective inverse problem solvers, acting as the prior of the distribution, while the information of the forward model can be granted at the sampling stage. Nonetheless, as the generative process remains in the same high dimensional (i.e. identical to data dimension) space, the models have not been extended to 3D inverse problems due to the extremely high memory and computational cost. In this paper, we combine the ideas from the conventional model-based iterative reconstruction with the modern diffusion models, which leads to a highly effective method for solving 3D medical image reconstruction tasks such as sparse-view tomography, limited angle tomography, compressed sensing MRI from pre-trained 2D diffusion models. In essence, we propose to augment the 2D diffusion prior with a model-based prior in the remaining direction at test time, such that one can achieve coherent reconstructions across all dimensions. Our method can be run in a single commodity GPU, and establishes the new state-of-the-art, showing that the proposed method can perform reconstructions of high fidelity and accuracy even in the most extreme cases (e.g. 2-view 3D tomography). We further reveal that the generalization capacity of the proposed method is surprisingly high, and can be used to reconstruct volumes that are entirely different from the training dataset. Code available: https://github.com/HJ-harry/DiffusionMBIR</details>  
- **Code**: [🔗](https://github.com/HJ-harry/DiffusionMBIR)

---
### Paper 21: [DiffusionMBIR](https://openaccess.thecvf.com/content/CVPR2023/papers/Chung_Solving_3D_Inverse_Problems_Using_Pre-Trained_2D_Diffusion_Models_CVPR_2023_paper.pdf)
- **Title**: Solving 3D Inverse Problems Using Pre-Trained 2D Diffusion Models  
- **Conference**: CVPR(2023)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  Integrates diffusion models with model-based iterative reconstruction to enable efficient and high-fidelity 3D medical image reconstruction from pre-trained 2D diffusion priors.  
- **Abstract**:  
  <details><summary>Click</summary>Diffusion models have emerged as the new state-of-the-art generative model with high quality samples, with intriguing properties such as mode coverage and high flexibility. They have also been shown to be effective inverse problem solvers, acting as the prior of the distribution, while the information of the forward model can be granted at the sampling stage. Nonetheless, as the generative process remains in the same high dimensional (i.e. identical to data dimension) space, the models have not been extended to 3D inverse problems due to the extremely high memory and computational cost. In this paper, we combine the ideas from the conventional model-based iterative reconstruction with the modern diffusion models, which leads to a highly effective method for solving 3D medical image reconstruction tasks such as sparse-view tomography, limited angle tomography, compressed sensing MRI from pre-trained 2D diffusion models. In essence, we propose to augment the 2D diffusion prior with a model-based prior in the remaining direction at test time, such that one can achieve coherent reconstructions across all dimensions. Our method can be run in a single commodity GPU, and establishes the new state-of-the-art, showing that the proposed method can perform reconstructions of high fidelity and accuracy even in the most extreme cases (e.g. 2-view 3D tomography). We further reveal that the generalization capacity of the proposed method is surprisingly high, and can be used to reconstruct volumes that are entirely different from the training dataset. Code available: https://github.com/HJ-harry/DiffusionMBIR </details>  
- **Code**: [🔗](https://github.com/HJ-harry/DiffusionMBIR)

---
### Paper 22: [C²RV](https://openaccess.thecvf.com/content/CVPR2024/papers/Lin_C2RV_Cross-Regional_and_Cross-View_Learning_for_Sparse-View_CBCT_Reconstruction_CVPR_2024_paper.pdf)
- **Title**: C²RV: Cross-Regional and Cross-View Learning for Sparse-View CBCT Reconstruction  
- **Conference**: CVPR(2024)  
- **Imaging**: CT  
- **Based on**: Volume  
- **Main Contribution**:  
  A multi-scale volumetric representation with scale-view cross-attention enables adaptive feature aggregation for improved 3D learning.  
- **Abstract**:  
  <details><summary>Click</summary> Cone beam computed tomography (CBCT) is an important imaging technology widely used in medical scenarios such as diagnosis and preoperative planning. Using fewer projection views to reconstruct CT also known as sparse-view reconstruction can reduce ionizing radiation and further benefit interventional radiology. Compared with sparse-view reconstruction for traditional parallel/fan-beam CT CBCT reconstruction is more challenging due to the increased dimensionality caused by the measurement process based on cone-shaped X-ray beams. As a 2D-to-3D reconstruction problem although implicit neural representations have been introduced to enable efficient training only local features are considered and different views are processed equally in previous works resulting in spatial inconsistency and poor performance on complicated anatomies. To this end we propose C^2RV by leveraging explicit multi-scale volumetric representations to enable cross-regional learning in the 3D space. Additionally the scale-view cross-attention module is introduced to adaptively aggregate multi-scale and multi-view features. Extensive experiments demonstrate that our C^2RV achieves consistent and significant improvement over previous state-of-the-art methods on datasets with diverse anatomy. Code is available at https://github.com/xmed-lab/C2RV-CBCT. </details>  
- **Code**: [🔗](https://github.com/xmed-lab/C2RV-CBCT)

---
### Paper 23: [Pezzotti et al.](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9241039)
- **Title**: An Adaptive Intelligence Algorithm for Undersampled Knee MRI Reconstruction  
- **Conference**: Access(2020)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  Adaptive intelligence enhances MRI reconstruction by integrating domain knowledge with deep learning, achieving top rankings in the fastMRI challenge.  
- **Abstract**:  
  <details><summary>Click</summary>Adaptive intelligence aims at empowering machine learning techniques with the additional use of domain knowledge. In this work, we present the application of adaptive intelligence to accelerate MR acquisition. Starting from undersampled k-space data, an iterative learning-based reconstruction scheme inspired by compressed sensing theory is used to reconstruct the images. We developed a novel deep neural network to refine and correct prior reconstruction assumptions given the training data. The network was trained and tested on a knee MRI dataset from the 2019 fastMRI challenge organized by Facebook AI Research and NYU Langone Health. All submissions to the challenge were initially ranked based on similarity with a known groundtruth, after which the top 4 submissions were evaluated radiologically. Our method was evaluated by the fastMRI organizers on an independent challenge dataset. It ranked #1, shared #1, and #3 on respectively the 8× accelerated multi-coil, the 4× multi-coil, and the 4× single-coil tracks. This demonstrates the superior performance and wide applicability of the method.</details>  
- **Code**: ❌

---
### Paper 24: [EMISR](https://www.sciencedirect.com/science/article/pii/S0169260719312416?casa_token=ccmALOmHwwEAAAAA:KiI5QXyplZ1HFNgEISLpq9V_wUtvmoOF7ZlectXzwYwRZ9rH4eIzdzq6BEM555v38SjolH81-g)
- **Title**: Super-resolution reconstruction of knee magnetic resonance imaging based on deep learning  
- **Conference**: CMBP(2020)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  Three hidden layers extracted from a super-resolution CNN are integrated with a sub-pixel convolution layer sourced from an efficient sub-pixel CNN.  
- **Abstract**:  
  <details><summary>Click</summary>Background and objective With the rapid development of medical imaging and intelligent diagnosis, artificial intelligence methods have become a research hotspot of radiography processing technology in recent years. The low definition of knee magnetic resonance image texture seriously affects the diagnosis of knee osteoarthritis. This paper presents a super-resolution reconstruction method to address this problem. Methods In this paper, we propose an efficient medical image super-resolution (EMISR) method, in which we mainly adopted three hidden layers of super-resolution convolution neural network (SRCNN) and a sub-pixel convolution layer of efficient sub-pixel convolution neural network (ESPCN). The addition of the efficient sub-pixel convolutional layer in the hidden layer and the small network replacement consisting of concatenated convolutions to address low-resolution images but not high-resolution images are important. The EMISR method also uses cascaded small convolution kernels to improve reconstruction speed and deepen the convolution neural network to improve reconstruction quality. Results The proposed method is tested in the public dataset IDI, and the reconstruction quality of the algorithm is higheJMIr than that of the sparse coding-based network (SCN) method, the SRCNN method, and the ESPCN method (+ 2.306 dB, + 2.540 dB, + 1.089 dB improved); moreover, the reconstruction speed is faster than its counterparts (+ 4.272 s, + 1.967 s, and + 0.073 s improved). Conclusion The experimental results show that our EMISR framework has improved performance and greatly reduces the number of parameters and training time. Furthermore, the reconstructed image presents more details, and the edges are more complete. Therefore, the EMISR technique provides a more powerful medical analysis in knee osteoarthritis examinations.</details>  
- **Code**: ❌

---
### Paper 25: [Shaul et al.](https://www.sciencedirect.com/science/article/pii/S1361841520301110)
- **Title**: Subsampled brain MRI reconstruction by generative adversarial neural networks  
- **Conference**: MIA(2020)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  High-quality MRI reconstruction is realized through the proposed framework by synergistically combining U-Net and GAN architectures.  
- **Abstract**:  
  <details><summary>Click</summary>A main challenge in magnetic resonance imaging (MRI) is speeding up scan time. Beyond improving patient experience and reducing operational costs, faster scans are essential for time-sensitive imaging, such as fetal, cardiac, or functional MRI, where temporal resolution is important and target movement is unavoidable, yet must be reduced. Current MRI acquisition methods speed up scan time at the expense of lower spatial resolution and costlier hardware. We introduce a practical, software-only framework, based on deep learning, for accelerating MRI acquisition, while maintaining anatomically meaningful imaging. This is accomplished by MRI subsampling followed by estimating the missing k-space samples via generative adversarial neural networks. A generator-discriminator interplay enables the introduction of an adversarial cost in addition to fidelity and image-quality losses used for optimizing the reconstruction. Promising reconstruction results are obtained from feasible sampling patterns of up to a fivefold acceleration of diverse brain MRIs, from a large publicly available dataset of healthy adult scans as well as multimodal acquisitions of multiple sclerosis patients and dynamic contrast-enhanced MRI (DCE-MRI) sequences of stroke and tumor patients. Clinical usability of the reconstructed MRI scans is assessed by performing either lesion or healthy tissue segmentation and comparing the results to those obtained by using the original, fully sampled images. Reconstruction quality and usability of the DCE-MRI sequences is demonstrated by calculating the pharmacokinetic (PK) parameters. The proposed MRI reconstruction approach is shown to outperform state-of-the-art methods for all datasets tested in terms of the peak signal-to-noise ratio (PSNR), the structural similarity index (SSIM), as well as either the mean squared error (MSE) with respect to the PK parameters, calculated for the fully sampled DCE-MRI sequences, or the segmentation compatibility, measured in terms of Dice scores and Hausdorff distance. The code is available on GitHub.</details>  
- **Code**: [🔗](https://github.com/ItamarDavid/Subsampled-Brain-MRI-Reconstruction-by-Generative-Adversarial-Neural-Networks.git)

---
### Paper 27: [MADGAN](https://link.springer.com/content/pdf/10.1186/s12859-020-03936-1.pdf)
- **Title**: MADGAN: unsupervised medical anomaly detection GAN using multiple adjacent brain MRI slice reconstruction  
- **Conference**: BMC Bioinformatics(2021)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  Propose a GAN-driven approach for reconstructing multiple adjacent brain MRI slices, enabling anomaly detection across different stages in multi-sequence structural MRI scans.  
- **Abstract**:  
  <details><summary>Click</summary>Background Unsupervised learning can discover various unseen abnormalities, relying on large-scale unannotated medical images of healthy subjects. Towards this, unsupervised methods reconstruct a 2D/3D single medical image to detect outliers either in the learned feature space or from high reconstruction loss. However, without considering continuity between multiple adjacent slices, they cannot directly discriminate diseases composed of the accumulation of subtle anatomical anomalies, such as Alzheimer’s disease (AD). Moreover, no study has shown how unsupervised anomaly detection is associated with either disease stages, various (i.e., more than two types of) diseases, or multi-sequence magnetic resonance imaging (MRI) scans. Results We propose unsupervised medical anomaly detection generative adversarial network (MADGAN), a novel two-step method using GAN-based multiple adjacent brain MRI slice reconstruction to detect brain anomalies at different stages on multi-sequence structural MRI: (Reconstruction) Wasserstein loss with Gradient Penalty + 100  loss—trained on 3 healthy brain axial MRI slices to reconstruct the next 3 ones—reconstructs unseen healthy/abnormal scans; (Diagnosis) Average  loss per scan discriminates them, comparing the ground truth/reconstructed slices. For training, we use two different datasets composed of 1133 healthy T1-weighted (T1) and 135 healthy contrast-enhanced T1 (T1c) brain MRI scans for detecting AD and brain metastases/various diseases, respectively. Our self-attention MADGAN can detect AD on T1 scans at a very early stage, mild cognitive impairment (MCI), with area under the curve (AUC) 0.727, and AD at a late stage with AUC 0.894, while detecting brain metastases on T1c scans with AUC 0.921. Conclusions Similar to physicians’ way of performing a diagnosis, using massive healthy training data, our first multiple MRI slice reconstruction approach, MADGAN, can reliably predict the next 3 slices from the previous 3 ones only for unseen healthy images. As the first unsupervised various disease diagnosis, MADGAN can reliably detect the accumulation of subtle anatomical anomalies and hyper-intense enhancing lesions, such as (especially late-stage) AD and brain metastases on multi-sequence MRI scans.</details>  
- **Code**: ❌

---
### Paper 28: [AUTOMAP](https://www.nature.com/articles/s41598-021-87482-7.pdf)
- **Title**: Boosting the signal-to-noise of low-field MRI with deep learning image reconstruction  
- **Conference**: Sci. report(2021)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  An end-to-end deep neural network framework is employed in to enhance the image quality of low-field MRI data severely degraded by noise.  
- **Abstract**:  
  <details><summary>Click</summary>Recent years have seen a resurgence of interest in inexpensive low magnetic field (< 0.3 T) MRI systems mainly due to advances in magnet, coil and gradient set designs. Most of these advances have focused on improving hardware and signal acquisition strategies, and far less on the use of advanced image reconstruction methods to improve attainable image quality at low field. We describe here the use of our end-to-end deep neural network approach (AUTOMAP) to improve the image quality of highly noise-corrupted low-field MRI data. We compare the performance of this approach to two additional state-of-the-art denoising pipelines. We find that AUTOMAP improves image reconstruction of data acquired on two very different low-field MRI systems: human brain data acquired at 6.5 mT, and plant root data acquired at 47 mT, demonstrating SNR gains above Fourier reconstruction by factors of 1.5- to 4.5-fold, and 3-fold, respectively. In these applications, AUTOMAP outperformed two different contemporary image-based denoising algorithms, and suppressed noise-like spike artifacts in the reconstructed images. The impact of domain-specific training corpora on the reconstruction performance is discussed. The AUTOMAP approach to image reconstruction will enable significant image quality improvements at low-field, especially in highly noise-corrupted environments.<details>  
- **Code**: ❌

---
### Paper 29: [CINE](https://www.nature.com/articles/s41598-020-70551-8.pdf)
- **Title**: CINENet: deep learning-based 3D cardiac CINE MRI reconstruction with multi-coil complex-valued 4D spatio-temporal convolutions  
- **Conference**: Sci.report(2020)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  A novel 4D deep reconstruction framework achieves efficient generation of high-quality isotropic 3D CINE MRI from single breath-hold acquisitions, demonstrating enhanced contrast and accelerated reconstruction.  
- **Abstract**:  
  <details><summary>Click</summary>Cardiac CINE magnetic resonance imaging is the gold-standard for the assessment of cardiac function. Imaging accelerations have shown to enable 3D CINE with left ventricular (LV) coverage in a single breath-hold. However, 3D imaging remains limited to anisotropic resolution and long reconstruction times. Recently deep learning has shown promising results for computationally efficient reconstructions of highly accelerated 2D CINE imaging. In this work, we propose a novel 4D (3D + time) deep learning-based reconstruction network, termed 4D CINENet, for prospectively undersampled 3D Cartesian CINE imaging. CINENet is based on (3 + 1)D complex-valued spatio-temporal convolutions and multi-coil data processing. We trained and evaluated the proposed CINENet on in-house acquired 3D CINE data of 20 healthy subjects and 15 patients with suspected cardiovascular disease. The proposed CINENet network outperforms iterative reconstructions in visual image quality and contrast (+ 67% improvement). We found good agreement in LV function (bias ± 95% confidence) in terms of end-systolic volume (0 ± 3.3 ml), end-diastolic volume (− 0.4 ± 2.0 ml) and ejection fraction (0.1 ± 3.2%) compared to clinical gold-standard 2D CINE, enabling single breath-hold isotropic 3D CINE in less than 10 s scan and ~ 5 s reconstruction time.</details>  
- **Code**: ❌

---
### Paper 30: [Recon3DMLP](https://arxiv.org/pdf/2301.08868)
- **Title**: Computationally Efficient 3D MRI Reconstruction with Adaptive MLP  
- **Conference**: MICCAI(2023)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  A hybrid of CNN modules with small kernels for low-frequency reconstruction and adaptive MLP modules with large kernels to boost the high-frequency reconstruction.  
- **Abstract**:  
  <details><summary>Click</summary>Compared with 2D MRI, 3D MRI provides superior volumetric spatial resolution and signal-to-noise ratio. However, it is more challenging to reconstruct 3D MRI images. Current methods are mainly based on convolutional neural networks (CNN) with small kernels, which are difficult to scale up to have sufficient fitting power for 3D MRI reconstruction due to the large image size and GPU memory constraint. Furthermore, MRI reconstruction is a deconvolution problem, which demands long-distance information that is difficult to capture by CNNs with small convolution kernels. The multi-layer perceptron (MLP) can model such long-distance information, but it requires a fixed input size. In this paper, we proposed Recon3DMLP, a hybrid of CNN modules with small kernels for low-frequency reconstruction and adaptive MLP (dMLP) modules with large kernels to boost the high-frequency reconstruction, for 3D MRI reconstruction. We further utilized the circular shift operation based on MRI physics such that dMLP accepts arbitrary image size and can extract global information from the entire FOV. We also propose a GPU memory efficient data fidelity module that can reduce >50% memory. We compared Recon3DMLP with other CNN-based models on a high-resolution (HR) 3D MRI dataset. Recon3DMLP improves HR 3D reconstruction and outperforms several existing CNN-based models under similar GPU memory consumption, which demonstrates that Recon3DMLP is a practical solution for HR 3D MRI reconstruction.</details>  
- **Code**: ❌

---
### Paper 31: [Li et al.](https://www.sciencedirect.com/science/article/abs/pii/S0169260724001068)
- **Title**: 3D-MRI super-resolution reconstruction using multi-modality based on multi-resolution CNN  
- **Conference**: CMPB(2024)  
- **Imaging**: MRI  
- **Based on**: Volume  
- **Main Contribution**:  
  A CNN based MRI super-resolution reconstruction method that integrates muti-resolution analysis and deep learning techniques in a way that is quite different from previous methods.  
- **Abstract**:  
  <details><summary>Click</summary>Background and ObjectiveHigh-resolution (HR) MR images provide rich structural detail to assist physicians in clinical diagnosis and treatment plan. However, it is arduous to acquire HR MRI due to equipment limitations, scanning time or patient comfort. Instead, HR MRI could be obtained through a number of computer assisted post-processing methods that have proven to be effective and reliable. This paper aims to develop a convolutional neural network (CNN) based super-resolutionreconstruction framework for low-resolution (LR) T2w images.MethodIn this paper, we propose a novel multi-modal HR MRI generation framework based on deep learning techniques. Specifically, we construct a CNN based on multi-resolution analysis to learn an end-to-end mapping between LR T2w and HR T2w, where HR T1w is fed into the network to offer detailed a priori information to help generate HR T2w. Furthermore, a low-frequency filtering module is introduced to filter out the interference from HR-T1w during high-frequency information extraction. Based on the idea of multi-resolution analysis, detailed features extracted from HR T1w and LR T2w are fused at two scales in the network and then HR T2w is reconstructed by upsampling and dense connectivity module.ResultsExtensive quantitative and qualitative evaluations demonstrate that the proposed method enhances the recovered HR T2w details and outperforms other state-of-the-art methods. In addition, the experimental results also suggest that our network has a lightweight structure and favorable generalization performance.ConclusionThe results show that the proposed method is capable of reconstructing HR T2w with higher accuracy. Meanwhile, the super-resolution reconstruction results on other dataset illustrate the excellent generalization ability of the method.</details>  
- **Code**: ❌

---
### Paper 32: [DirectPet](https://www.spiedigitallibrary.org/journals/journal-of-medical-imaging/volume-7/issue-3/032503/DirectPET--full-size-neural-network-PET-reconstruction-from-sinogram/10.1117/1.JMI.7.3.032503.full)
- **Title**: DirectPET: full-size neural network PET reconstruction from sinogram data  
- **Conference**: JMI(2020)  
- **Imaging**: PET  
- **Based on**: Volume  
- **Main Contribution**:  
  DirectPET introduces an efficient neural network with a Radon inversion layer for fast, high-quality multislice PET reconstruction from sinograms.  
- **Abstract**:  
  <details><summary>Click</summary>Purpose: Neural network image reconstruction directly from measurement data is a relatively new field of research, which until now has been limited to producing small single-slice images (e.g., 1  ×  128  ×  128). We proposed a more efficient network design for positron emission tomography called DirectPET, which is capable of reconstructing multislice image volumes (i.e., 16  ×  400  ×  400) from sinograms. Approach: Large-scale direct neural network reconstruction is accomplished by addressing the associated memory space challenge through the introduction of a specially designed Radon inversion layer. Using patient data, we compare the proposed method to the benchmark ordered subsets expectation maximization (OSEM) algorithm using signal-to-noise ratio, bias, mean absolute error, and structural similarity measures. In addition, line profiles and full-width half-maximum measurements are provided for a sample of lesions. Results: DirectPET is shown capable of producing images that are quantitatively and qualitatively similar to the OSEM target images in a fraction of the time. We also report on an experiment where DirectPET is trained to map low-count raw data to normal count target images, demonstrating the method’s ability to maintain image quality under a low-dose scenario. Conclusion: The ability of DirectPET to quickly reconstruct high-quality, multislice image volumes suggests potential clinical viability of the method. However, design parameters and performance boundaries need to be fully established before adoption can be considered.[/details]  
- **Code**: ❌

---
### Paper 33: [DLE](https://link.springer.com/content/pdf/10.1007/s00259-021-05478-x.pdf)
- **Title**: Image enhancement of whole-body oncology [18F]-FDG PET scans using deep neural networks to reduce noise  
- **Conference**: EJNMMI(2022)  
- **Imaging**: PET  
- **Based on**: Volume  
- **Main Contribution**:  
  Deep learning-based enhancement improves oncology 18F-FDG PET scan quality, enabling shorter scan and reconstruction times while preserving accuracy.  
- **Abstract**:  
  <details><summary>Click</summary>Purpose To enhance the image quality of oncology [18F]-FDG PET scans acquired in shorter times and reconstructed by faster algorithms using deep neural networks. Methods List-mode data from 277 [18F]-FDG PET/CT scans, from six centres using GE Discovery PET/CT scanners, were split into ¾-, ½- and ¼-duration scans. Full-duration datasets were reconstructed using the convergent block sequential regularised expectation maximisation (BSREM) algorithm. Short-duration datasets were reconstructed with the faster OSEM algorithm. The 277 examinations were divided into training (n = 237), validation (n = 15) and testing (n = 25) sets. Three deep learning enhancement (DLE) models were trained to map full and partial-duration OSEM images into their target full-duration BSREM images. In addition to standardised uptake value (SUV) evaluations in lesions, liver and lungs, two experienced radiologists scored the quality of testing set images and BSREM in a blinded clinical reading (175 series).ResultsOSEM reconstructions demonstrated up to 22% difference in lesion SUVmax, for different scan durations, compared to full-duration BSREM. Application of the DLE models reduced this difference significantly for full-, ¾- and ½-duration scans, while simultaneously reducing the noise in the liver. The clinical reading showed that the standard DLE model with full- or ¾-duration scans provided an image quality substantially comparable to full-duration scans with BSREM reconstruction, yet in a shorter reconstruction time. Conclusion Deep learning–based image enhancement models may allow a reduction in scan time (or injected activity) by up to 50%, and can decrease reconstruction time to a third, while maintaining image quality.</details>  
- **Code**: ❌

---
### Paper 34: [Deidda1 et al.](https://link.springer.com/content/pdf/10.1186/s40658-023-00549-4.pdf)
- **Title**: Triple modality image reconstruction of PET data using SPECT, PET, CT information increases lesion uptake in images of patients treated with radioembolization with 90 Y micro-spheres  
- **Conference**: EJNMMI(2023)  
- **Imaging**: CT PET SPECT  
- **Based on**: Volume  
- **Main Contribution**:  
  A triple-modality PET/SPECT/CT reconstruction method is proposed to enhance PET image quality, significantly improving lesion uptake quantification for theranostic applications.  
- **Abstract**:  
  <details><summary>Click</summary>Purpose Nuclear medicine imaging modalities like computed tomography (CT), single photon emission CT (SPECT) and positron emission tomography (PET) are employed in the field of theranostics to estimate and plan the dose delivered to tumors and the surrounding tissues and to monitor the effect of the therapy. However, therapeutic radionuclides often provide poor images, which translate to inaccurate treatment planning and inadequate monitoring images. Multimodality information can be exploited in the reconstruction to enhance image quality. Triple modality PET/SPECT/CT scanners are particularly useful in this context due to the easier registration process between images. In this study, we propose to include PET, SPECT and CT information in the reconstruction of PET data. The method is applied to Yttrium-90 (90Y) data.MethodsData from a NEMA phantom filled with 90Y were used for validation. PET, SPECT and CT data from 10 patients treated with Selective Internal Radiation Therapy (SIRT) were used. Different combinations of prior images using the Hybrid kernelized expectation maximization were investigated in terms of VOI activity and noise suppression.ResultsOur results show that triple modality PET reconstruction provides significantly higher uptake when compared to the method used as standard in the hospital and OSEM. In particular, using CT-guided SPECT images, as guiding information in the PET reconstruction significantly increases uptake quantification on tumoral lesions.ConclusionThis work proposes the first triple modality reconstruction method and demonstrates up to 69% lesion uptake increase over standard methods with SIRT 90Y patient data. Promising results are expected for other radionuclide combination used in theranostic applications using PET and SPECT.</details>  
- **Code**: [🔗](https://github.com/UCL/STIR.git)

---
### Paper 35: [Hashimoto et al.](https://arxiv.org/pdf/2212.11844)
- **Title**: Fully 3D implementation of the end-to-end deep image prior-based PET image reconstruction using block iterative algorithm  
- **Conference**: PMB(2023)  
- **Imaging**: PET  
- **Based on**: Volume  
- **Main Contribution**:  
  A shape-aware diffusion model for 3D image reconstruction from limited 2D images, incorporating shape priors to enhance topologyble.  
- **Abstract**:  
  <details><summary>Click</summary>Objective. Deep image prior (DIP) has recently attracted attention owing to its unsupervised positron emission tomography (PET) image reconstruction method, which does not require any prior training dataset. In this paper, we present the first attempt to implement an end-to-end DIP-based fully 3D PET image reconstruction method that incorporates a forward-projection model into a loss function. Approach. A practical implementation of a fully 3D PET image reconstruction could not be performed at present because of a graphics processing unit memory limitation. Consequently, we modify the DIP optimization to a block iteration and sequential learning of an ordered sequence of block sinograms. Furthermore, the relative difference penalty (RDP) term is added to the loss function to enhance the quantitative accuracy of the PET image. Main results. We evaluated our proposed method using Monte Carlo simulation with [18F]FDG PET data of a human brain and a preclinical study on monkey-brain [18F]FDG PET data. The proposed method was compared with the maximum-likelihood expectation maximization (EM), maximum a posteriori EM with RDP, and hybrid DIP-based PET reconstruction methods. The simulation results showed that, compared with other algorithms, the proposed method improved the PET image quality by reducing statistical noise and better preserved the contrast of brain structures and inserted tumors. In the preclinical experiment, finer structures and better contrast recovery were obtained with the proposed method. Significance. The results indicated that the proposed method could produce high-quality images without a prior training dataset. Thus, the proposed method could be a key enabling technology for the straightforward and practical implementation of end-to-end DIP-based fully 3D PET image reconstruction.</details>  
- **Code**: ❌

---
### Paper 36: [Gong et al. ](https://papers.miccai.org/miccai-2024/paper/3664_paper.pdf)
- **Title**: PET Image Denoising Based on 3D Denoising Diffusion Probabilistic Model: Evaluations on Total-Body Datasets  
- **Conference**: MICCAI(2024)  
- **Imaging**: PET  
- **Based on**: Volume  
- **Main Contribution**:  
  Proposes and evaluates denoising diffusion probabilistic model based methods for PET image denoising, demonstrating that incorporating PET and MRI priors improves performance over traditional denoising approaches.  
- **Abstract**:  
  <details><summary>Click</summary>Due to various physical degradation factors and limited photon counts detected, obtaining high-quality images from low-dose Positron emission tomography (PET) scans is challenging. The Denoising Diffusion Probabilistic Model (DDPM), an advanced distribution learning-based generative model, has shown promising performance across various computer-vision tasks. However, currently DDPM is mainly investigated in 2D mode, which has limitations for PET image denoising, as PET is usually acquired, reconstructed, and analyzed in 3D mode. In this work, we proposed a 3D DDPM method for PET image denoising, which employed a 3D convolutional network to train the score function, enabling the network to learn 3D distribution. The total-body -FDG PET datasets acquired from the Siemens Biograph Vision Quadra scanner (axial field of view > 1 m) were employed to evaluate the 3D DDPM method, as these total-body datasets needed 3D operations the most to leverage the rich information from different axial slices. All models were trained on 1/20 low-dose images and then evaluated on 1/4, 1/20, and 1/50 low-dose images, respectively. Experimental results indicated that 3D DDPM significantly outperformed 2D DDPM and 3D UNet in qualitative and quantitative assessments, capable of recovering finer structures and more accurate edge contours from low-quality PET images. Moreover, 3D DDPM revealed greater robustness when there were noise level mismatches between training and testing data. Finally, comparing 3D DDPM with 2D DDPM in terms of uncertainty revealed 3D DDPM’s higher confidence in reproducibility.</details>  
- **Code**: ❌

---
### Paper 37: [Mostafapour et al.](https://www.hug.ch/sites/interhug/files/structures/pinlab/documents/jcde2022.pdf)
- **Title**: Deep learning-guided attenuation correction in the image domain for myocardial perfusion SPECT imaging  
- **Conference**: JCDE(2022)  
- **Imaging**: SPECT  
- **Based on**: Volume  
- **Main Contribution**:  
  Using residual and UNet deep convolutional neural networks, it investigates the accuracy of direct attenuation correction in the image domain for myocardial perfusion SPECT imaging.  
- **Abstract**:  
  <details><summary>Click</summary>We investigate the accuracy of direct attenuation correction (AC) in the image domain for myocardial perfusion SPECT (single-photon emission computed tomography) imaging (MPI-SPECT) using residual (ResNet) and UNet deep convolutional neural networks. MPI-SPECT 99mTc-sestamibi images of 99 patients were retrospectively included. UNet and ResNet networks were trained using non-attenuation-corrected SPECT images as input, whereas CT-based attenuation-corrected (CT-AC) SPECT images served as reference. Chang’s calculated AC approach considering a uniform attenuation coefficient within the body contour was also implemented. Clinical and quantitative evaluations of the proposed methods were performed considering SPECT CT-AC images of 19 subjects (external validation set) as reference. Image-derived metrics, including the voxel-wise mean error (ME), mean absolute error, relative error, structural similarity index (SSI), and peak signal-to-noise ratio, as well as clinical relevant indices, such as total perfusion deficit (TPD), were utilized. Overall, AC SPECT images generated using the deep learning networks exhibited good agreement with SPECT CT-AC images, substantially outperforming Chang’s method. The ResNet and UNet models resulted in an ME of −6.99 ± 16.72 and −4.41 ± 11.8 and an SSI of 0.99 ± 0.04 and 0.98 ± 0.05, respectively. Chang’s approach led to ME and SSI of 25.52 ± 33.98 and 0.93 ± 0.09, respectively. Similarly, the clinical evaluation revealed a mean TPD of 12.78 ± 9.22% and 12.57 ± 8.93% for ResNet and UNet models, respectively, compared to 12.84 ± 8.63% obtained from SPECT CT-AC images. Conversely, Chang’s approach led to a mean TPD of 16.68 ± 11.24%. The deep learning AC methods have the potential to achieve reliable AC in MPI-SPECT imaging.</details>  
- **Code**: ❌

---
### Paper 38: [TPL-CNN](https://link.springer.com/content/pdf/10.1186/s40658-024-00687-3.pdf)
- **Title**: SPECT-MPI iterative denoising during the reconstruction process using a two-phase learned convolutional neural network  
- **Conference**: EJNMMI(2024)  
- **Imaging**: SPECT  
- **Based on**: Volume  
- **Main Contribution**:  
  An iterative deep denoising method using a GAN-based approach improves SPECT myocardial perfusion imaging by reducing noise and enhancing contrast during reconstruction.  
- **Abstract**:  
  <details><summary>Click</summary>Purpose The problem of image denoising in single-photon emission computed tomography (SPECT) myocardial perfusion imaging (MPI) is a fundamental challenge. Although various image processing techniques have been presented, they may degrade the contrast of denoised images. The proposed idea in this study is to use a deep neural network as the denoising procedure during the iterative reconstruction process rather than the post-reconstruction phase. This method could decrease the background coefficient of variation (COV_bkg) of the final reconstructed image, which represents the amount of random noise, while improving the contrast-to-noise ratio (CNR).MethodsIn this study, a generative adversarial network is used, where its generator is trained by a two-phase approach. In the first phase, the network is trained by a confined image region around the heart in transverse view. The second phase improves the network’s generalization by tuning the network weights with the full image size as the input. The network was trained and tested by a dataset of 247 patients who underwent two immediate serially high- and low-noise SPECT-MPI.ResultsQuantitative results show that compared to post-reconstruction low pass filtering and post-reconstruction deep denoising methods, our proposed method can decline the COV_bkg of the images by up to 10.28% and 12.52% and enhance the CNR by up to 54.54% and 45.82%, respectively.ConclusionThe iterative deep denoising method outperforms 2D low-pass Gaussian filtering with an 8.4-mm FWHM and post-reconstruction deep denoising approaches.</details>  
- **Code**: [🔗](https://github.com/FYousefzadeh/in-house-simple-OSEM2D-code.git)

---
### Paper 39: [Li et al.](https://arxiv.org/pdf/2312.15676)
- **Title**: Sparse-view CT Reconstruction with 3D Gaussian Volumetric Representation  
- **Conference**: arxiv(2024)  
- **Imaging**: CT  
- **Based on**: GR  
- **Main Contribution**:  
  A self-supervised 3D Gaussian method using FBP priors and adaptive updates for efficient sparse-view CT reconstruction.  
- **Abstract**:  
  <details><summary>Click</summary>Sparse-view CT is a promising strategy for reducing the radiation dose of traditional CT scans, but reconstructing high-quality images from incomplete and noisy data is challenging. Recently, 3D Gaussian has been applied to model complex natural scenes, demonstrating fast convergence and better rendering of novel views compared to implicit neural representations (INRs). Taking inspiration from the successful application of 3D Gaussians in natural scene modeling and novel view synthesis, we investigate their potential for sparse-view CT reconstruction. We leverage prior information from the filtered-backprojection reconstructed image to initialize the Gaussians; and update their parameters via comparing difference in the projection space. Performance is further enhanced by adaptive density control. Compared to INRs, 3D Gaussians benefit more from prior information to explicitly bypass learning in void spaces and allocate the capacity efficiently, accelerating convergence. 3D Gaussians also efficiently learn high-frequency details. Trained in a self-supervised manner, 3D Gaussians avoid the need for large-scale paired data. Our experiments on the AAPM-Mayo dataset demonstrate that 3D Gaussians can provide superior performance compared to INR-based methods. This work is in progress, and the code will be publicly available.</detais>  
- **Code**: ❌

---
### Paper 40: [DIF-Gaussian](https://arxiv.org/pdf/2407.01090)
- **Title**: Learning 3D Gaussians for Extremely Sparse-View Cone-Beam CT Reconstruction  
- **Conference**: MICCAI(2024)  
- **Imaging**: CT  
- **Based on**: GR  
- **Main Contribution**:  
  A framework for sparse-view CBCT reconstruction using 3D Gaussian features and test-time optimization to improve anatomical imaging.  
- **Abstract**:  
  <details><summary>Click</summary>Cone-Beam Computed Tomography (CBCT) is an indispensable technique in medical imaging, yet the associated radiation exposure raises concerns in clinical practice. To mitigate these risks, sparse-view reconstruction has emerged as an essential research direction, aiming to reduce the radiation dose by utilizing fewer projections for CT reconstruction. Although implicit neural representations have been introduced for sparse-view CBCT reconstruction, existing methods primarily focus on local 2D features queried from sparse projections, which is insufficient to process the more complicated anatomical structures, such as the chest. To this end, we propose a novel reconstruction framework, namely DIF-Gaussian, which leverages 3D Gaussians to represent the feature distribution in the 3D space, offering additional 3D spatial information to facilitate the estimation of attenuation coefficients. Furthermore, we incorporate test-time optimization during inference to further improve the generalization capability of the model. We evaluate DIF-Gaussian on two public datasets, showing significantly superior reconstruction performance than previous state-of-the-art methods. The code is available at https://github.com/xmed-lab/DIF-Gaussian.</detais>  
- **Code**: [🔗](https://github.com/xmed-lab/DIF-Gaussian)

---
### Paper 41: [R²-Gaussian](https://arxiv.org/pdf/2405.20693)
- **Title**: R2-Gaussian: Rectifying Radiative Gaussian Splatting for Tomographic Reconstruction  
- **Conference**: NeurIPS(2024)  
- **Imaging**: CT  
- **Based on**: GR  
- **Main Contribution**:  
  A novel 3D Gaussian splatting framework that rectifies integration bias for rapid, accurate sparse-view tomographic reconstruction.  
- **Abstract**:  
  <details><summary>Click</summary>  3D Gaussian splatting (3DGS) has shown promising results in image rendering and surface reconstruction. However, its potential in volumetric reconstruction tasks, such as X-ray computed tomography, remains under-explored. This paper introduces R2-Gaussian, the first 3DGS-based framework for sparse-view tomographic reconstruction. By carefully deriving X-ray rasterization functions, we discover a previously unknown integration bias in the standard 3DGS formulation, which hampers accurate volume retrieval. To address this issue, we propose a novel rectification technique via refactoring the projection from 3D to 2D Gaussians. Our new method presents three key innovations: (1) introducing tailored Gaussian kernels, (2) extending rasterization to X-ray imaging, and (3) developing a CUDA-based differentiable voxelizer. Experiments on synthetic and real-world datasets demonstrate that our method outperforms state-of-the-art approaches in accuracy and efficiency. Crucially, it delivers high-quality results in 4 minutes, which is 12× faster than NeRF-based methods and on par with traditional algorithms. Code and models are available on the project page this https URL.</details>  
- **Code**: [🔗](https://github.com/Ruyi-Zha/r2_gaussian.git)

---
### Paper 42: [GaSpCT](https://arxiv.org/pdf/2404.03126)
- **Title**: GaSpCT: Gaussian Splatting for Novel CT Projection View Synthesis  
- **Conference**: MICCAI(2024)  
- **Imaging**: CT  
- **Based on**: GR  
- **Main Contribution**:  
  GaSpCT synthesizes CT views from limited 2D images without SfM reducing scan time and enhancing foreground–background separation  
- **Abstract**:  
  <details><summary>Click</summary> We present GaSpCT, a novel view synthesis and 3D scene representation method used to generate novel projection views for Computer Tomography (CT) scans. We adapt the Gaussian Splatting framework to enable novel view synthesis in CT based on limited sets of 2D image projections and without the need for Structure from Motion (SfM) methodologies. Therefore, we reduce the total scanning duration and the amount of radiation dose the patient receives during the scan. We adapted the loss function to our use-case by encouraging a stronger background and foreground distinction using two sparsity promoting regularizers: a beta loss and a total variation (TV) loss. Finally, we initialize the Gaussian locations across the 3D space using a uniform prior distribution of where the brain's positioning would be expected to be within the field of view. We evaluate the performance of our model using brain CT scans from the Parkinson's Progression Markers Initiative (PPMI) dataset and demonstrate that the rendered novel views closely match the original projection views of the simulated scan, and have better performance than other implicit 3D scene representations methodologies. Furthermore, we empirically observe reduced training time compared to neural network based image synthesis for sparse-view CT image reconstruction. Finally, the memory requirements of the Gaussian Splatting representations are reduced by 17% compared to the equivalent voxel grid image representations.</details>  
- **Code**: ❌

---
### Paper 43: [DDGS-CT](https://proceedings.neurips.cc/paper_files/paper/2024/file/456ce0476c9b4689a74918b851cecd5a-Paper-Conference.pdf)
- **Title**: DDGS-CT: Direction-Disentangled Gaussian Splatting  for Realistic Volume Rendering  
- **Conference**: NeurIPS(2024)  
- **Imaging**: CT  
- **Based on**: GR  
- **Main Contribution**:  
  A direction-disentangled 3D Gaussian splatting framework for efficient, differentiable DRR generation modeling anisotropic X-ray effects for intraoperative imaging.  
- **Abstract**:  
  <details><summary>Click</summary>Digitally reconstructed radiographs (DRRs) are simulated 2D X-ray images generated from 3D CT volumes, widely used in preoperative settings but limited in intraoperative applications due to computational bottlenecks, especially for accurate but heavy physics-based Monte Carlo methods. While analytical DRR renderers offer greater efficiency, they overlook anisotropic X-ray image formation phenomena, such as Compton scattering. We present a novel approach that marries realistic physics-inspired X-ray simulation with efficient, differentiable DRR generation using 3D Gaussian splatting (3DGS). Our direction-disentangled 3DGS (DDGS) method separates the radiosity contribution into isotropic and direction-dependent components, approximating complex anisotropic interactions without intricate runtime simulations. Additionally, we adapt the 3DGS initialization to account for tomography data properties, enhancing accuracy and efficiency. Our method outperforms state-of-the-art techniques in image accuracy. Furthermore, our DDGS shows promise for intraoperative applications and inverse problems such as pose registration, delivering superior registration accuracy and runtime performance compared to analytical DRR methods.</details>  
- **Code**: ❌

---
### Paper 44: [X-Gaussain](https://arxiv.org/pdf/2403.04116)
- **Title**: Radiative Gaussian Splatting for Efficient X-Ray Novel View Synthesis  
- **Conference**: ECCV(2024)  
- **Imaging**: CT  
- **Based on**: GR  
- **Main Contribution**:  
  A 3D Gaussian splatting-based framework for efficient, high-quality novel X-ray view synthesis and rapid sparse-view CT reconstruction.  
- **Abstract**:  
  <details><summary>Click</summary>X-ray is widely applied for transmission imaging due to its stronger penetration than natural light. When rendering novel view X-ray projections, existing methods mainly based on NeRF suffer from long training time and slow inference speed. In this paper, we propose a 3D Gaussian splatting-based method, namely X-Gaussian, for X-ray novel view synthesis. Firstly, we redesign a radiative Gaussian point cloud model inspired by the isotropic nature of X-ray imaging. Our model excludes the influence of view direction when learning to predict the radiation intensity of 3D points. Based on this model, we develop a Differentiable Radiative Rasterization (DRR) with CUDA implementation. Secondly, we customize an Angle-pose Cuboid Uniform Initialization (ACUI) strategy that directly uses the parameters of the X-ray scanner to compute the camera information and then uniformly samples point positions within a cuboid enclosing the scanned object. Experiments show that our X-Gaussian outperforms state-of-the-art methods by 6.5 dB while enjoying less than 15% training time and over 73 inference speed. The application on CT reconstruction also reveals the practical values of our method. Code is at https://github.com/caiyuanhao1998/X-Gaussian.</details>  
- **Code**: [🔗](https://github.com/caiyuanhao1998/X-Gaussian)

---
### Paper 45: [GBIR](https://openreview.net/pdf?id=AkCWbxntll)
- **Title**: GBIR: A Novel Gaussian Iterative Method for Medical Image Reconstruction  
- **Conference**: ICLR(2025)  
- **Imaging**: PET  
- **Based on**: GR  
- **Main Contribution**:  
  A Gaussian-Based Iterative Reconstruction framework that leverages learnable Gaussians for personalized CT and MRI reconstruction from undersampled data, overcoming deep learning limitations and validated on the MORE  
- **Abstract**:  
  <details><summary>Click</summary>Computed Tomography (CT) and Magnetic Resonance Imaging (MRI) are crucial diagnostic tools, but undersampling techniques like Sparse-View CT (SV-CT) and Compressed-Sensing MRI (CS-MRI), aimed at reducing patient exposure and scan time, make image reconstruction more challenging. While deep learning-based reconstruction (DLR) methods have made significant strides, they face limitations in adapting to varying scan geometries and handling diverse patient data, hindering widespread clinical use. In this paper, we propose a novel Gaussian-Based Iterative Reconstruction (GBIR) framework that uses learnable Gaussians representations for personalized medical image reconstruction, addressing the shortcomings of DLR methods. GBIR optimizes case-specific parameters in an end-to-end fashion, enabling better generalization and flexibility under sparse measurements. Additionally, we introduce the Multi-Organ Medical Image REconstruction (MORE) dataset, comprising over 70,000 CT and MRI slices across multiple body parts and conditions. Our experiments show that GBIR outperforms state-of-the-art methods in both accuracy and speed, offering a robust solution for personalized medical image reconstruction.</details>  
- **Code**: ❌

---
### Paper 46: [PINER](https://openaccess.thecvf.com/content/WACV2023/papers/Song_PINER_Prior-Informed_Implicit_Neural_Representation_Learning_for_Test-Time_Adaptation_in_WACV_2023_paper.pdf)
- **Title**: PINER: Prior-informed Implicit Neural Representation Learning for Test-time  Adaptation in Sparse-view CT Reconstruction  
- **Conference**: WACV (2023)  
- **Imaging**: CT  
- **Based on**: IPE  
- **Main Contribution**:  
  A novel source-free black-box test-time adaptation approach via prior-informed implicit neural representation learning for sparse-view CT reconstruction with unknown noise levels.  
- **Abstract**:  
  <details><summary>Click</summary>Recently, deep learning has been introduced to solve important medical image reconstruction problems such as sparse-view CT reconstruction. However, the developed deep reconstruction models are generally limited in generalization when applied to unseen testing samples in target domain. Furthermore, privacy concerns may impede the availability of source-domain training data to retrain or adapt the model to the target-domain testing data, which are quite common in real-world medical applications. To address these issues, we introduce a source-free black-box test-time adaptation method for sparse-view CT reconstruction with unknown noise levels based on prior-informed implicit neural representation learning (PINER). By leveraging implicit neural representation learning to generate the image representations at various noise levels, the proposed method is able to construct the adapted input representations at test time based on the inference of black-box model and output analysis. We performed experiments of source-free test-time adaptation for sparse-view CT reconstruction with unknown noise levels on multiple anatomical sites with different black-box deep reconstruction models, where our method outperforms the state-of-the-art algorithms. </details>  
- **Code**: [🔗](https://github.com/efzero/PINER)

---
### Paper 47: [GONG et al.](https://www.researchgate.net/profile/Kuang-Gong/publication/352643894_Direct_Reconstruction_of_Linear_Parametric_Images_from_Dynamic_PET_Using_Nonlocal_Deep_Image_Prior/links/60d4900f299bf1fe469b2deb/Direct-Reconstruction-of-Linear-Parametric-Images-from-Dynamic-PET-Using-Nonlocal-Deep-Image-Prior.pdf)
- **Title**: Direct Reconstruction of Linear Parametric Images From Dynamic PET Using Nonlocal Deep Image Prior  
- **Conference**: TMI(2022)  
- **Imaging**: PET  
- **Based on**: IPE  
- **Main Contribution**:  
  An unsupervised deep learning framework for dynamic PET parametric reconstruction, using 3D U-Net with embedded kinetic model as a convolution layer.  
- **Abstract**:  
  <details><summary>Click</summary>Direct reconstruction methods have been developed to estimate parametric images directly from the measured PET sinograms by combining the PET imaging model and tracer kinetics in an integrated framework. Due to limited counts received, signal-to-noise-ratio (SNR) and resolution of parametric images produced by direct reconstruction frameworks are still limited. Recently supervised deep learning methods have been successfully applied to medical imaging denoising/reconstruction when large number of high-quality training labels are available. For static PET imaging, high-quality training labels can be acquired by extending the scanning time. However, this is not feasible for dynamic PET imaging, where the scanning time is already long enough. In this work, we proposed an unsupervised deep learning framework for direct parametric reconstruction from dynamic PET, which was tested on the Patlak model and the relative equilibrium Logan model. The training objective function was based on the PET statistical model. The patient’s anatomical prior image, which is readily available from PET/CT or PET/MR scans, was supplied as the network input to provide a manifold constraint, and also utilized to construct a kernel layer to perform non-local feature denoising. The linear kinetic model was embedded in the network structure as a 1×1×1 convolution layer. Evaluations based on dynamic datasets of 18F-FDG and 11C-PiB tracers show that the proposed framework can outperform the traditional and the kernel method-based direct reconstruction methods.</details>  
- **Code**: ❌

---
### Paper 48: [Makkar et al.](https://www.iccr2024.org/papers/526223.pdf)
- **Title**: Partial-ring PET Image Correction using Implicit Neural Representation Learning  
- **Conference**: ICCR(2024)  
- **Imaging**: PET  
- **Based on**: IPE NRF  
- **Main Contribution**:  
  A deep learning-based approach enhances image quality in partial-ring PET scanners using implicit neural representation learning with coordinate-based MLPs.  
- **Abstract**:  
  <details><summary>Click</summary>This work introduces a deep learning-based approach to enhance image quality in partial-ring PET scanners,which often suffer from significant artifacts due to incomplete angular field of view. Our method utilizes implicit neural representation (INR) learning with coordinate-based multilayer perceptrons (MLPs) featuring sinusoidal activations. These MLPs parameterize partial-ring PET images, training the patientspecific network to predict fully sampled images from partially sampled ones. This approach was validated using twenty digital brain phantoms, Monte Carlo simulated Derenzo phantom, and experimentally acquired hot rod phantom data from the partial-ring PETITION PET scanner. The results show that the INR learning method significantly improves image quality, achieving a PSNR above 30dB and SSIM over 0.95 for all cases. This method presents a promising solution for enhancing PET images from partial-ring scanners.</details>  
- **Code**: ❌

---
### Paper 49: [NeRP](https://med.stanford.edu/content/dam/sm/dbds/XingSR1.pdf)
- **Title**: NeRP: Implicit Neural Representation Learning with Prior Embedding for Sparsely Sampled Image Reconstruction  
- **Conference**: TNNLS(2022)  
- **Imaging**: CT MRI  
- **Based on**: IPE  
- **Main Contribution**:  
  An implicit neural representation learning methodology integrating longitudinal information into deep learning models with anatomical information as the image prior for reconstructing computational images from sparse measurements.  
- **Abstract**:  
  <details><summary>Click</summary>Image reconstruction is an inverse problem that solves for a computational image based on sampled sensor measurement. Sparsely sampled image reconstruction poses additional challenges due to limited measurements. In this work, we propose a methodology of implicit Neural Representation learning with Prior embedding (NeRP) to reconstruct a computational image from sparsely sampled measurements. The method differs fundamentally from previous deep learning-based image reconstruction approaches in that NeRP exploits the internal information in an image prior and the physics of the sparsely sampled measurements to produce a representation of the unknown subject. No large-scale data is required to train the NeRP except for a prior image and sparsely sampled measurements. In addition, we demonstrate that NeRP is a general methodology that generalizes to different imaging modalities such as computed tomography (CT) and magnetic resonance imaging (MRI). We also show that NeRP can robustly capture the subtle yet significant image changes required for assessing tumor progression. </details>  
- **Code**: [🔗]( https://github.com/liyues/NeRP)

---
### Paper 50: [Liu et al.](https://www.pure.ed.ac.uk/ws/portalfiles/portal/482363230/LiuEtalIEEETMI2024Geometry-awareAttenuationLearning.pdf)
- **Title**: Geometry-Aware Attenuation Learning for Sparse-View CBCT Reconstruction  
- **Conference**: TMI(2025)  
- **Imaging**: CT MRI  
- **Based on**: IPE  
- **Main Contribution**:  
  A geometry-aware encoder-decoder framework for sparse use-view CBCT reconstruction by leveraging the prior knowledge and back-projecting multiview 2D features into 3D space.  
- **Abstract**:  
  <details><summary>Click</summary>Cone Beam Computed Tomography (CBCT) plays a vital role in clinical imaging. Traditional methods typically require hundreds of 2D X-ray projections to reconstruct a high-quality 3D CBCT image, leading to considerable radiation exposure. This has led to a growing interest in sparse-view CBCT reconstruction to reduce radiation doses. While recent advances, including deep learning and neural rendering algorithms, have made strides in this area, these methods either produce unsatisfactory results or suffer from time inefficiency of individual optimization. In this paper, we introduce a novel geometry-aware encoder-decoder framework to solve this problem. Our framework starts by encoding multi-view 2D features from various 2D X-ray projections with a 2D CNN encoder. Leveraging the geometry of CBCT scanning, it then back-projects the multi-view 2D features into the 3D space to formulate a comprehensive volumetric feature map, followed by a 3D CNN decoder to recover 3D CBCT image. Importantly, our approach respects the geometric relationship between 3D CBCT image and its 2D X-ray projections during feature back projection stage, and enjoys the prior knowledge learned from the data population. This ensures its adaptability in dealing with extremely sparse view inputs without individual training, such as scenarios with only 5 or 10 X-ray projections. Extensive evaluations on two simulated datasets and one real-world dataset demonstrate exceptional reconstruction quality and time efficiency of our method.</details>  
- **Code**: ❌

---
### Paper 51: [Ultra-NeRF](https://proceedings.mlr.press/v227/wysocki24a/wysocki24a.pdf)
- **Title**: Ultra-NeRF: Neural Radiance Fields for Ultrasound Imaging  
- **Conference**: MIDC（2024）  
- **Imaging**: 3D US  
- **Based on**: NRF  
- **Main Contribution**:  
  A ray-tracing-based method for synthesizing accurate B-mode images by learning view-dependent scene appearance and geometry from multiple US sweeps.  
- **Abstract**:  
  <details><summary>Click</summary>We present a physics-enhanced implicit neural representation (INR) for ultrasound (US) imaging that learns tissue properties from overlapping US sweeps. Our proposed method leverages a ray-tracing-based neural rendering for novel view US synthesis. Recent publications demonstrated that INR models could encode a representation of a three-dimensional scene from a set of two-dimensional US frames. However, these models fail to consider the view-dependent changes in appearance and geometry intrinsic to US imaging. In our work, we discuss direction-dependent changes in the scene and show that a physics-inspired rendering improves the fidelity of US image synthesis. In particular, we demonstrate experimentally that our proposed method generates geometrically accurate B-mode images for regions with ambiguous representation owing to view-dependent differences of the US images. We conduct our experiments using simulated B-mode US sweeps of the liver and acquired US sweeps of a spine phantom tracked with a robotic arm. The experiments corroborate that our method generates US frames that enable consistent volume compounding from previously unseen views. To the best of our knowledge, the presented work is the first to address view-dependent US image synthesis using INR.</details>  
- **Code**: ❌

---
### Paper 52: [UlRe-NeRF](https://arxiv.org/pdf/2408.00860)
- **Title**: UlRe-NeRF: 3D Ultrasound Imaging through  Neural Rendering with Ultrasound Reflection  Direction Parameterization  
- **Conference**: arXiv(2024)  
- **Imaging**: 3D US  
- **Based on**: NRF  
- **Main Contribution**:  
  A ultrasound neural rendering model integrating implicit neural networks and explicit volume rendering, featuring reflection direction parameterization and harmonic encoding.  
- **Abstract**:  
  <details><summary>Click</summary>Three-dimensional ultrasound imaging is a critical technology widely used in medical diagnostics. However, traditional 3D ultrasound imaging methods have limitations such as fixed resolution, low storage efficiency, and insufficient contextual connectivity, leading to poor performance in handling complex artifacts and reflection characteristics. Recently, techniques based on NeRF (Neural Radiance Fields) have made significant progress in view synthesis and 3D reconstruction, but there remains a research gap in high-quality ultrasound imaging. To address these issues, we propose a new model, UlRe-NeRF, which combines implicit neural networks and explicit ultrasound volume rendering into an ultrasound neural rendering architecture. This model incorporates reflection direction parameterization and harmonic encoding, using a directional MLP module to generate view-dependent high-frequency reflection intensity estimates, and a spatial MLP module to produce the medium's physical property parameters. These parameters are used in the volume rendering process to accurately reproduce the propagation and reflection behavior of ultrasound waves in the medium. Experimental results demonstrate that the UlRe-NeRF model significantly enhances the realism and accuracy of high-fidelity ultrasound image reconstruction, especially in handling complex medium structures. </details>  
- **Code**: ❌

---
### Paper 53: [NeRF-US](https://arxiv.org/pdf/2408.10258)
- **Title**: NeRF-US: Removing Ultrasound Imaging Artifacts from Neural Radiance Fields in the Wild  
- **Conference**: arXiv(2024)  
- **Imaging**: 3D US  
- **Based on**: NRF  
- **Main Contribution**:  
  An approach for training NeRFs on ultrasound imaging that incorporates the properties of ultrasound imaging and incorporates 3D priors through a diffusion model, also utilizing ultrasound-specific rendering.  
- **Abstract**:  
  <details><summary>Click</summary>Current methods for performing 3D reconstruction and novel view synthesis (NVS) in ultrasound imaging data often face severe artifacts when training NeRF-based approaches. The artifacts produced by current approaches differ from NeRF floaters in general scenes because of the unique nature of ultrasound capture. Furthermore, existing models fail to produce reasonable 3D reconstructions when ultrasound data is captured or obtained casually in uncontrolled environments, which is common in clinical settings. Consequently, existing reconstruction and NVS methods struggle to handle ultrasound motion, fail to capture intricate details, and cannot model transparent and reflective surfaces. In this work, we introduced NeRF-US, which incorporates 3D-geometry guidance for border probability and scattering density into NeRF training, while also utilizing ultrasound-specific rendering over traditional volume rendering. These 3D priors are learned through a diffusion model. Through experiments conducted on our new "Ultrasound in the Wild" dataset, we observed accurate, clinically plausible, artifact-free reconstructions. </details>  
- **Code**: [🔗](rishitdagli.com/nerf-us/)

---
### Paper 54: [ImplicitVol](https://arxiv.org/pdf/2109.12108)
- **Title**: ImplicitVol: Sensorless 3D Ultrasound Reconstruction with Deep Implicit Representation  
- **Conference**: arXiv(2021)  
- **Imaging**: 3D US  
- **Based on**: NRF  
- **Main Contribution**:  
  A model for deep implicit 3D volume sensorless reconstruction from 2D freehand ultrasound images, featuring implicit spatial-to-intensity mapping.  
- **Abstract**:  
  <details><summary>Click</summary>The objective of this work is to achieve sensorless reconstruction of a 3D volume from a set of 2D freehand ultrasound images with deep implicit representation. In contrast to the conventional way that represents a 3D volume as a discrete voxel grid, we do so by parameterizing it as the zero level-set of a continuous function, i.e. implicitly representing the 3D volume as a mapping from the spatial coordinates to the corresponding intensity values. Our proposed model, termed as ImplicitVol, takes a set of 2D scans and their estimated locations in 3D as input, jointly refining the estimated 3D locations and learning a full reconstruction of the 3D volume. When testing on real 2D ultrasound images, novel cross-sectional views that are sampled from ImplicitVol show significantly better visual quality than those sampled from existing reconstruction approaches, outperforming them by over 30% (NCC and SSIM), between the output and ground-truth on the 3D volume testing data. The code will be made publicly available. </details>  
- **Code**: ❌

---
### Paper 55: [MedNeRF](https://arxiv.org/pdf/2202.01020)
- **Title**: MedNeRF: Medical Neural Radiance Fields for Reconstructing 3D-aware CT-Projections from a Single X-ray  
- **Conference**: EMBC(2022)  
- **Imaging**: CT  
- **Based on**: NRF  
- **Main Contribution**:  
  A novel NeRF-based deep learning architecture for continuous CT scan representation from a few single-view X-ray.  
- **Abstract**:  
  <details><summary>Click</summary>Computed tomography (CT) is an effective med-ical imaging modality, widely used in the field of clinical medicine for the diagnosis of various pathologies. Advances in Multidetector CT imaging technology have enabled additional functionalities, including generation of thin slice multi planar cross-sectional body imaging and 3D reconstructions. However, this involves patients being exposed to a considerable dose of ionising radiation. Excessive ionising radiation can lead to deterministic and harmful effects on the body. This paper proposes a Deep Learning model that learns to reconstruct CT projections from a few or even a single-view X-ray. This is based on a novel architecture that builds from neural radiance fields, which learns a continuous representation of CT scans by disentangling the shape and volumetric depth of surface and internal anatomical structures from 2D images. Our model is trained on chest and knee datasets, and we demonstrate qual-itative and quantitative high-fidelity renderings and compare our approach to other recent radiance field-based methods. Our code and link to our datasets are available at https://qithub.com/abrilcf/mednerf Clinical relevance- Our model is able to infer the anatomical 3D structure from a few or a single-view X-ray showing future potential for reduced ionising radiation exposure during the imaging process. </details>  
- **Code**: [🔗](https://github.com/abrilcf/mednerf)

---
### Paper 56: [NAF](https://arxiv.org/pdf/2209.14540)
- **Title**: Neural Attenuation Fields for Sparse-View  CBCT Reconstruction  
- **Conference**: MICCAI (2022)  
- **Imaging**: CT  
- **Based on**: NRF  
- **Main Contribution**:  
  NAF advances  self-supervised sparse-view CBCT reconstruction without external training data.  
- **Abstract**:  
  <details><summary>Click</summary>This paper proposes a novel and fast self-supervised solution for sparse-view CBCT reconstruction (Cone Beam Computed Tomography) that requires no external training data. Specifically, the desired attenuation coefficients are represented as a continuous function of 3D spatial coordinates, parameterized by a fully-connected deep neural network. We synthesize projections discretely and train the network by minimizing the error between real and synthesized projections. A learning-based encoder entailing hash coding is adopted to help the network capture high-frequency details. This encoder outperforms the commonly used frequency-domain encoder in terms of having higher performance and efficiency, because it exploits the smoothness and sparsity of human organs. Experiments have been conducted on both human organ and phantom datasets. The proposed method achieves state-of-the-art accuracy and spends reasonably short computation time. </details>  
- **Code**: [🔗](https://github.com/Ruyi-Zha/naf_cbct)

---
### Paper 57: [DIF-Net](https://arxiv.org/pdf/2303.06681)
- **Title**: Learning Deep Intensity Field for Extremely  Sparse-View CBCT Reconstruction  
- **Conference**: MICCAI (2023)  
- **Imaging**: CT  
- **Based on**: IPE  
- **Main Contribution**:  
  A supervised CBCT reconstruction framework for high-quality, high-resolution CBCT from $\leq10$ sparse views.  
- **Abstract**:  
  <details><summary>Click</summary>Sparse-view cone-beam CT (CBCT) reconstruction is an important direction to reduce radiation dose and benefit clinical applications. Previous voxel-based generation methods represent the CT as discrete voxels, resulting in high memory requirements and limited spatial resolution due to the use of 3D decoders. In this paper, we formulate the CT volume as a continuous intensity field and develop a novel DIF-Net to perform high-quality CBCT reconstruction from extremely sparse (≤10) projection views at an ultrafast speed. The intensity field of a CT can be regarded as a continuous function of 3D spatial points. Therefore, the reconstruction can be reformulated as regressing the intensity value of an arbitrary 3D point from given sparse projections. Specifically, for a point, DIF-Net extracts its view-specific features from different 2D projection views. These features are subsequently aggregated by a fusion module for intensity estimation. Notably, thousands of points can be processed in parallel to improve efficiency during training and testing. In practice, we collect a knee CBCT dataset to train and evaluate DIF-Net. Extensive experiments show that our approach can reconstruct CBCT with high image quality and high spatial resolution from extremely sparse views within 1.6 s, significantly outperforming state-of-the-art methods. Our code will be available at https://github.com/xmed-lab/DIF-Net. </details>  
- **Code**: [🔗](https://github.com/xmed-lab/DIF-Net)

---
### Paper 58: [ACnerf](https://iopscience.iop.org/article/10.1088/1361-6560/ad1d6c/meta)
- **Title**: ACnerf: enhancement of neural radiance field by alignment and correction of pose to reconstruct new views from a single x-ray*  
- **Conference**: PMB(2024)  
- **Imaging**: CT  
- **Based on**: NRF  
- **Main Contribution**:  
  ACnerf improves NeRF-based single-view X-ray CT reconstruction by enhancing alignment, pose correction, and rendering precision.  
- **Abstract**:  
  <details><summary>Click</summary>Objective. Computed tomography (CT) is widely used in medical research and clinical diagnosis. However, acquiring CT data requires patients to be exposed to considerable ionizing radiance, leading to physical harm. Recent studies have considered using neural radiance field (NERF) techniques to infer the full-view CT projections from single-view x-ray projection, thus aiding physician judgment and reducing Radiance hazards. This paper enhances this technique in two directions: (1) accurate generalization capabilities for control models. (2) Consider different ranges of viewpoints. Approach. Building upon generative radiance fields (GRAF), we propose a method called ACnerf to enhance the generalization of the NERF through alignment and pose correction. ACnerf aligns with a reference single x-ray by utilizing a combination of positional encoding with Gaussian random noise (latent code) obtained from GRAF training. This approach avoids compromising the 3D structure caused by altering the generator. During inference, a pose judgment network is employed to correct the pose and optimize the rendered viewpoint. Additionally, when generating a narrow range of views, ACnerf employs frequency-domain regularization to fine-tune the generator and achieve precise projections. Main results. The proposed ACnerf method surpasses the state-of-the-art NERF technique in terms of rendering quality for knee and chest data with varying contrasts. It achieved an average improvement of 2.496 dB in PSNR and 41% in LPIPS for 0°–360° projections. Additionally, for −15° to 15° projections, ACnerf achieved an average improvement of 0.691 dB in PSNR and 25.8% in LPIPS. Significance. With adjustments in alignment, inference, and rendering range, our experiments and evaluations on knee and chest data of different contrasts show that ACnerf effectively reduces artifacts and aberrations in the new view. ACnerf's ability to recover more accurate 3D structures from single x-rays has excellent potential for reducing damage from ionising radiation in clinical diagnostics.</details>  
- **Code**: ❌

---
### Paper 59: [UMedNeRF](https://arxiv.org/pdf/2311.05836)
- **Title**: UMedNeRF: Uncertainty-Aware Single View Volumetric Rendering For Medical Neural Radiance Fields  
- **Conference**: ISBI(2024)  
- **Imaging**: CT  
- **Based on**: NRF  
- **Main Contribution**:  
  A radiance field-based network for continuous CT projection representation from 2D X-rays, with internal structure extraction and multi-task loss optimization.  
- **Abstract**:  
  <details><summary>Click</summary>In the field of clinical medicine, computed tomography (CT) is an effective medical imaging modality for the diagnosis of various pathologies. Compared with X-ray images, CT images can provide more information, including multi-planar slices and three-dimensional structures for clinical diagnosis. However, CT imaging requires patients to be exposed to large doses of ionizing radiation for a long time, which may cause irreversible physical harm. In this paper, we propose an Uncertainty-aware MedNeRF (UMedNeRF) network based on generated radiation fields. This network can learn a continuous representation of CT projections from 2D X-ray images by obtaining the internal structure and depth information and using multi-task adaptive loss weights to ensure the quality of the generated images. Our model is trained on publicly available knee and chest datasets, and we show the results of CT projection rendering with a single X-ray and compare our method with other methods based on generated radiation fields. </details>  
- **Code**: ❌

---
### Paper 60: [VolumeNeRF](https://papers.miccai.org/miccai-2024/paper/3061_paper.pdf)
- **Title**: VolumeNeRF: CT Volume Reconstruction from a Single Projection View  
- **Conference**: MICCAI (2024)  
- **Imaging**: CT  
- **Based on**: NRF  
- **Main Contribution**:  
  VolumeNeRF reconstructs CT volumes from a single-view X-ray using NeRF with anatomical priors and a projection attention module.  
- **Abstract**:  
  <details><summary>Click</summary>Computed tomography (CT) plays a significant role in clinical practice by providing detailed three-dimensional information, aiding in accurate assessment of various diseases. However, CT imaging requires a large number of X-ray projections from different angles and exposes patients to high doses of radiation. Here we propose VolumeNeRF, based on neural radiance fields (NeRF), for reconstructing CT volumes from a single-view X-ray. During training, our network learns to generate a continuous representation of the CT scan conditioned on the input X-ray image and render an X-ray image similar to the input from the same viewpoint as the input. Considering the ill-posedness and the complexity of the single-perspective generation task, we introduce likelihood images and the average CT images to incorporate prior anatomical knowledge. A novel projection attention module is designed to help the model learn the spatial correspondence between voxels in CT images and pixels in X-ray images during the imaging process. Extensive experiments conducted on a publicly available chest CT dataset show that our VolumeNeRF achieves better performance than other state-of-the-art methods. Our code is available at https://www.github.com/Aurora132/VolumeNeRF. </details>  
- **Code**: [🔗](https://www.github.com/Aurora132/VolumeNeRF)

---
### Paper 61: [SAX-NeRF](https://openaccess.thecvf.com/content/ICCV2023/papers/Chen_CuNeRF_Cube-Based_Neural_Radiance_Field_for_Zero-Shot_Medical_Image_Arbitrary-Scale_ICCV_2023_paper.pdf)
- **Title**: Structure-Aware Sparse-View X-ray 3D Reconstruction  
- **Conference**: CVPR(2024)  
- **Imaging**: CT  
- **Based on**: NRF  
- **Main Contribution**:  
  SAX-NeRF improves sparse-view X-ray 3D reconstruction by introducing Lineformer for structural modeling and Masked Local-Global ray sampling for enhanced feature extraction.  
- **Abstract**:  
  <details><summary>Click</summary> X-ray known for its ability to reveal internal structures of objects is expected to provide richer information for 3D reconstruction than visible light. Yet existing NeRF algorithms overlook this nature of X-ray leading to their limitations in capturing structural contents of imaged objects. In this paper we propose a framework Structure-Aware X-ray Neural Radiodensity Fields (SAX-NeRF) for sparse-view X-ray 3D reconstruction. Firstly we design a Line Segment-based Transformer (Lineformer) as the backbone of SAX-NeRF. Linefomer captures internal structures of objects in 3D space by modeling the dependencies within each line segment of an X-ray. Secondly we present a Masked Local-Global (MLG) ray sampling strategy to extract contextual and geometric information in 2D projection. Plus we collect a larger-scale dataset X3D covering wider X-ray applications. Experiments on X3D show that SAX-NeRF surpasses previous NeRF-based methods by 12.56 and 2.49 dB on novel view synthesis and CT reconstruction. https://github.com/caiyuanhao1998/SAX-NeRF</details>  
- **Code**: [🔗](https://github.com/caiyuanhao1998/SAX-NeRF)

---
### Paper 62: [extended-MedNeRF](https://www.biorxiv.org/content/10.1101/2023.04.24.538160v1.full.pdf)
- **Title**: 3D reconstructions of brain from MRI scans using neural radiance fields  
- **Conference**: AISC (2023)  
- **Imaging**: MRI  
- **Based on**: NRF  
- **Main Contribution**:  
  A neural radiance field-based approach for reconstructing 3D projections from 2D MRI slices.  
- **Abstract**:  
  <details><summary>Click</summary>The advent of 3D Magnetic Resonance Imaging (MRI) has revolutionized medical imaging and diagnostic capabilities, allowing for more precise diagnosis, treatment planning, and improved patient outcomes. 3D MRI imaging enables the creation of detailed 3D reconstructions of anatomical structures that can be used for visualization, analysis, and surgical planning. However, these reconstructions often require many scan acquisitions, demanding a long session to use the machine and requiring the patient to remain still, with consequent possible motion artifacts. The development of neural radiance fields (NeRF) technology has shown promising results in generating highly accurate 3D reconstructions of MRI images with less user input. Our approach is based on neural radiance fields to reconstruct 3D projections from 2D slices of MRI scans. We do this by using 3D convolutional neural networks to address challenges posed by variable slice thickness; incorporating multiple MRI modalities to ensure robustness and extracting the shape and volumetric depth of both surface and internal anatomical structures with slice interpolation. This approach provides more comprehensive and robust 3D reconstructions of both surface and internal anatomical structures and has significant potential for clinical applications, allowing medical professionals to better visualize and analyze anatomical structures with less available data, potentially reducing times and motion-related issues. </details>  
- **Code**: ❌

---
### Paper 63: [Feng et al.](https://arxiv.org/pdf/2301.00127)
- **Title**: Spatiotemporal implicit neural representation for unsupervised dynamic MRI reconstruction  
- **Conference**: TMI(2025)  
- **Imaging**: CT MRI  
- **Based on**: NRF  
- **Main Contribution**:  
  An INR-based unsupervised deep learning approach that reconstructs dynamic MRI from highly undersampled k-space data using only spatiotemporal coordinate inputs.  
- **Abstract**:  
  <details><summary>Click</summary>Supervised Deep-Learning (DL)-based reconstruction algorithms have shown state-of-the-art results for highly-undersampled dynamic Magnetic Resonance Imaging (MRI) reconstruction. However, the requirement of excessive high-quality ground-truth data hinders their applications due to the generalization problem. Recently, Implicit Neural Representation (INR) has emerged as a powerful DL-based tool for solving the inverse problem by characterizing the attributes of a signal as a continuous function of corresponding coordinates in an unsupervised manner. In this work, we proposed an INR-based method to improve dynamic MRI reconstruction from highly undersampled k-space data, which only takes spatiotemporal coordinates as inputs and does not require any training on external datasets or transfer-learning from prior images. Specifically, the proposed method encodes the dynamic MRI images into neural networks as an implicit function, and the weights of the network are learned from sparsely-acquired (k, t)-space data itself only. Benefiting from the strong implicit continuity regularization of INR together with explicit regularization for low-rankness and sparsity, our proposed method outperforms the compared state-of-the-art methods at various acceleration factors. E.g., experiments on retrospective cardiac cine datasets show an improvement of 0.6–2.0 dB in PSNR for high accelerations (up to 40.8×). The high-quality and inner continuity of the images provided by INR exhibit great potential to further improve the spatiotemporal resolution of dynamic MRI. The code is available at: https://github.com/AMRILab/INR_for_DynamicMRI. </details>  
- **Code**: [🔗]( https://github.com/AMRILab/INR_for_DynamicMRI)

---
### Paper 64: [NeSVoR](https://www.researchgate.net/profile/Junshen-Xu/publication/365043351_NeSVoR_Implicit_Neural_Representation_for_Slice-to-Volume_Reconstruction_in_MRI/links/636ab7c5431b1f53007e10d9/NeSVoR-Implicit-Neural-Representation-for-Slice-to-Volume-Reconstruction-in-MRI.pdf)
- **Title**: NeSVoR: Implicit Neural Representation for Slice-to-Volume Reconstruction in MRI  
- **Conference**: TMI (2023)  
- **Imaging**: CT MRI  
- **Based on**: NRF  
- **Main Contribution**:  
  A resolution-agnostic slice-to-volume reconstruction framework that represents the underlying volume as a continuous spatial function using implicit neural representation.  
- **Abstract**:  
  <details><summary>Click</summary>Reconstructing 3D MR volumes from multiple motion-corrupted stacks of 2D slices has shown promise in imaging of moving subjects, e. g., fetal MRI. However, existing slice-to-volume reconstruction methods are time-consuming, especially when a high-resolution volume is desired. Moreover, they are still vulnerable to severe subject motion and when image artifacts are present in acquired slices. In this work, we present NeSVoR, a resolution-agnostic slice-to-volume reconstruction method, which models the underlying volume as a continuous function of spatial coordinates with implicit neural representation. To improve robustness to subject motion and other image artifacts, we adopt a continuous and comprehensive slice acquisition model that takes into account rigid inter-slice motion, point spread function, and bias fields. NeSVoR also estimates pixel-wise and slice-wise variances of image noise and enables removal of outliers during reconstruction and visualization of uncertainty. Extensive experiments are performed on both simulated and in vivo data to evaluate the proposed method. Results show that NeSVoR achieves state-of-the-art reconstruction quality while providing two to ten-fold acceleration in reconstruction times over the state-of-the-art algorithms. </details>  
- **Code**: [🔗](https://github.com/daviddmc/NeSVoR)

---
### Paper 65: [CuNeRF](https://openaccess.thecvf.com/content/ICCV2023/papers/Chen_CuNeRF_Cube-Based_Neural_Radiance_Field_for_Zero-Shot_Medical_Image_Arbitrary-Scale_ICCV_2023_paper.pdf)
- **Title**: CuNeRF: Cube-Based Neural Radiance Field for Zero-Shot Medical Image Arbitrary-Scale Super Resolution  
- **Conference**: ICCV(2023)  
- **Imaging**: CT MRI  
- **Based on**: NRF  
- **Main Contribution**:  
  A zero-shot medical image super-resolution framework that generates high-quality images at arbitrary scales and viewpoints without requiring high-resolution training data.  
- **Abstract**:  
  <details><summary>Click</summary> Medical image arbitrary-scale super-resolution (MIASSR) has recently gained widespread attention, aiming to supersample medical volumes at arbitrary scales via a single model. However, existing MIASSR methods face two major limitations: (i) reliance on high-resolution (HR) volumes and (ii) limited generalization ability, which restricts their applications in various scenarios. To overcome these limitations, we propose Cube-based Neural Radiance Field (CuNeRF), a zero-shot MIASSR framework that is able to yield medical images at arbitrary scales and free viewpoints in a continuous domain. Unlike existing MISR methods that only fit the mapping between low-resolution (LR) and HR volumes, CuNeRF focuses on building a continuous volumetric representation from each LR volume without the knowledge from the corresponding HR one. This is achieved by the proposed differentiable modules: cube-based sampling, isotropic volume rendering, and cube-based hierarchical rendering. Through extensive experiments on magnetic resource imaging (MRI) and computed tomography (CT) modalities, we demonstrate that CuNeRF can synthesize high-quality SR medical images, which outperforms state-of-the-art MISR methods, achieving better visual verisimilitude and fewer objectionable artifacts. Compared to existing MISR methods, our CuNeRF is more applicable in practice.</details>  
- **Code**: [🔗](NarcissusEx.github.io/CuNeRF)

---
### Paper 66: [RAO et al.](https://ieeexplore.ieee.org/abstract/document/10004486)
- **Title**: An Energy-Efficient Accelerator for Medical Image  Reconstruction From Implicit Neural Representation  
- **Conference**: TCAS-I(2022)  
- **Imaging**: CT MRI  
- **Based on**: NRF  
- **Main Contribution**:  
  An energy-efficient accelerator with co-designed hardware architecture for Implicit Neural Representation (INR)-based medical image reconstruction, optimizing both data reuse patterns and computational load distribution.  
- **Abstract**:  
  <details><summary>Click</summary>This work presents an energy-efficient accelerator for medical image reconstruction from implicit neural representation (INR). The accelerator implements an INR-based algorithm to deliver high-quality medical image reconstruction with arbitrary resolution from a compact implicit format. In particular, we propose a dedicated hardware architecture based on an optimized computation flow for the INR-based reconstruction algorithm, which co-designs data reuse and computation load. The proposed architecture takes in the coordinate of the intersection of three scans and outputs all the voxel intensities, minimizing the data movement between on-chip and off-chip. To validate the proposed accelerator, we build a proof-of-concept prototype demonstration system using field programmable gate array (FPGA). We also map our design to 40nm CMOS technology to measure the performance of the proposed accelerator. The implementation results show that, running at 400MHz, the proposed accelerator is capable of processing medical images with 256×256 resolution in real-time at 26.3 frames per second (FPS), with a power consumption of only 795 mW. Comparison results show that the performance, as well as the energy efficiency of the proposed accelerator, outperforms the central processing unit (CPU)-based and graphic processing unit (GPU)-based implementations. </details> 
- **Code**: ❌
