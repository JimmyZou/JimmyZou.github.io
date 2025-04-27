# Blog Medical Image AI Related

---
## Contents
 - [Medical Image AI](#medical-image-ai)

---


## Medical Image AI

### [Nature Biomedical Engineering 2017] Surgical data science for next-generation interventions [[PDF]](https://www.nature.com/articles/s41551-017-0132-7)
_Lena Maier-Hein, Swaroop S. Vedula, Stefanie Speidel, Nassir Navab, Ron Kikinis, Adrian Park, Matthias Eisenmann, Hubertus Feussner, Germain Forestier, Stamatia Giannarou, Makoto Hashizume, Darko Katic, Hannes Kenngott, Michael Kranzfelder, Anand Malpani, Keno März, Thomas Neumuth, Nicolas Padoy, Carla Pugh, Nicolai Schoch, Danail Stoyanov, Russell Taylor, Martin Wagner, Gregory D. Hager & Pierre Jannin_

### [MICCAI 2024] Depth-Driven Geometric Prompt Learning for Laparoscopic Liver Landmark Detection [[PDF]](https://www.arxiv.org/abs/2406.17858)
_Jialun Pei, Ruize Cui, Yaoqian Li, Weixin Si, Jing Qin, Pheng-Ann Heng_
- ![](../assets/fig_medical/1.png)

### Multi-resolution 3d convolutional neural networks for automatic coronary centerline extraction in cardiac ct angiography scans

### Coronary artery centerline extraction in cardiac ct angiography using a cnn-based orientation classifier [[code]](https://github.com/BubblyYi/Coronary-Artery-Tracking-via-3D-CNN-Classification)

### VesselNet: A deep convolutional neural network with multi pathways for robust hepatic vessel segmentation

### DeepVesselNet: Vessel Segmentation, Centerline Prediction, and Bifurcation Detection in 3-D Angiographic Volumes

---

## Text-promptable segmentation

### [NeurIPS 2023] Text Promptable Surgical Instrument Segmentation with Vision-Language Models
- Our model leverages multiple text prompts for each surgical instrument through a new mixture of prompts mechanism, resulting in enhanced segmentation performance. Additionally, we introduce a hard instrument area reinforcement module to improve image feature comprehension and segmentation precision.

### [arXiv 2023] AdaptiveSAM: Towards Efficient Tuning of SAM for Surgical Scene Segmentation
- We propose AdaptiveSAM - an adaptive modification of SAM that can adjust to new datasets quickly and efficiently, while enabling text-prompted segmentation.
- report the average object-wise DICE Scores and IoU scores across the four test datasets
- RESULTS ON ENDOVIS 18. BG TISSUE - BACKGROUND TISSUE, RI - ROBOTIC INSTRUMENT, KP - KIDNEY PARENNCHYMA, CK - COVERED
KIDNEY, SN - SUTURING NEEDLE, SUCTION INS. - SUCTION INSTRUMENT, S. INTESTINE - SMALL INTESTINE, UP - ULTRASOUND PROBE


## Non-text promptable segmentation

### [TIP 2024] Boundary-Aware Prototype in Semi-Supervised Medical Image Segmentation
- Inspired by this, we propose a novel consistency learning framework based on the non-parametric distance metric of boundary-aware prototypes to alleviate this problem.
- Boundary-Aware Prototype Segmentation
- LA Dataset, Pancreas-NIH Dataset

### [arXiv 2023] Medical SAM Adapter: Adapting Segment Anything Model for Medical Image Segmentation
- following the official ViT-H SAM GitHub repository
- For the REFUGE2, TNMIX, and ISIC datasets, we trained the model for 40 epochs. For the BTCV and BraTs datasets, we extended the training to 60 epochs.

### [AAAI 2024] SurgicalSAM: Efficient Class Promptable Surgical Instrument Segmentation
- To address these problems, we introduce SurgicalSAM, a novel end-to-end efficient-tuning approach for SAM to effectively integrate surgical-specific information with SAM's pre-trained knowledge for improved generalisation. Specifically, we propose a lightweight prototype-based class prompt encoder for tuning, which directly generates prompt embeddings from class prototypes and eliminates the use of explicit prompts for improved robustness and a simpler pipeline. In addition, to address the low inter-class variance among surgical instrument categories, we propose contrastive prototype learning, further enhancing the discrimination of the class prototypes for more accurate class prompting. 
- The results of extensive experiments on both EndoVis2018 and EndoVis2017 datasets demonstrate that SurgicalSAM achieves state-of-the-art performance while only requiring a small number of tunable parameters.

### [NeurIPS 2024 Workshop] Surgical SAM 2: Real-time segment anything in surgical video by efficient frame pruning

### [arXiv 2024] Medical SAM 2: Segment medical images as video via Segment Anything Model 2

### [Nature Method 2023] Towards foundation models of biological image segmentation

---

## Survey

### [arXiv 2024] Segment Anything Model for Medical Image Segmentation: Current Applications and Future Directions

### [MIA 2025] Medical SAM Adapter: Adapting Segment Anything Model for Medical Image Segmentation

### [TMI 2024] Video-instrument synergistic network for referring video instrument segmentation in robotic surgery

### [CVPR 2024] One-Prompt to Segment All Medical Images

### [AAAI 2024] Medsegdiff-v2: Diffusion based medical image segmentation with transformer

### [TMI 2022] Exploring Intra- and Inter-Video Relation for Surgical Semantic Scene Segmentation

### [Nature Communications 2024] Segment Anything in Medical Images


---
