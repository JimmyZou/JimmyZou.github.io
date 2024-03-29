# Blog Generative Models Related

---
## Contents
 - [Fundation Models](#fundation-models)


---
## Summary of multi-modal alignment methods

- video-text contrastive learning
- masked video modeling
- next token prediction
- a joint visual-audio-text representation 
- knowledge distill


---
## Fundation Models

### [!!!] [Meta AI] Segment Anything [[pdf]](https://arxiv.org/abs/2304.02643)
_Alexander Kirillov, Eric Mintun, Nikhila Ravi, Hanzi Mao, Chloe Rolland, Laura Gustafson, Tete Xiao, Spencer Whitehead, Alexander C. Berg, Wan-Yen Lo, Piotr Dollár, Ross Girshick_
- We take inspiration from NLP, where the next token prediction task is used for foundation model pre-training and to solve diverse downstream tasks via prompt engineering.
- Task generalization vs multi-task segmentation
- MAE pre-trained Vision Transformer (ViT)
- The data engine has three stages: (1) a model-assisted manual annotation stage, (2) a semi-automatic stage with a mix of automatically predicted masks and model-assisted annotation, and (3) a fully automatic stage in which our model generates masks without annotator input.
- Specifically, we prompt SAM to (1) perform edge detection, (2) segment everything, i.e. object proposal generation, (3) segment detected objects, i.e. instance segmentation, and (4), as a proof-of-concept, to segment objects from free-form text. These four tasks differ significantly from the promptable segmentation task that SAM was trained on and are implemented via prompt engineering.
- ![](../assets/fig_generative_models/8.png)
- ![](../assets/fig_generative_models/9.png)

### [!!!] [arXiv 2024] Stable Video Diffusion: Scaling Latent Video Diffusion Models to Large Datasets [[pdf]](https://arxiv.org/abs/2311.15127)
_Andreas Blattmann, Tim Dockhorn, Sumith Kulal, Daniel Mendelevitch, Maciej Kilian, Dominik Lorenz, Yam Levi, Zion English, Vikram Voleti, Adam Letts, Varun Jampani, Robin Rombach_
- In this paper, we identify and evaluate three different stages for successful training of video LDMs: text-to-image pretraining, video pretraining, and high-quality video finetuning. 
- We demonstrate the necessity of a well-curated pretraining dataset.
- Our model provides a strong multi-view 3D-prior.
- Our model provides a powerful motion representation for downstream tasks such as image-to-video generation and adaptability to camera motion-specific LoRA modules.

### [!!!] [OpenAI] CLIP: Learning transferable visual models from natural language supervision [[pdf]](https://arxiv.org/abs/2103.00020)
_Alec Radford, Jong Wook Kim, Chris Hallacy, Aditya Ramesh, Gabriel Goh, Sandhini Agarwal, Girish Sastry, Amanda Askell, Pamela Mishkin, Jack Clark, Gretchen Krueger, Ilya Sutskever_
- ![](../assets/fig_generative_models/10.png)
- To address this, we constructed a new dataset of 400 million (image, text) pairs collected form a variety of publicly available sources on the Internet. To attempt to cover as broad a set of visual concepts as possible, we search for (image, text) pairs as part of the construction process whose text includes one of a set of 500,000 queries. We approximately class balance the results by including up to 20,000 (image, text) pairs per query. The resulting dataset has a similar total word count as the WebText dataset used to train GPT-2. We refer to this dataset as WIT for WebImageText.

### [ICML 2021] ALIGN: Scaling up visual and vision-language representation learning with noisy text supervision [[pdf]](https://arxiv.org/abs/2102.05918)
_Chao Jia, Yinfei Yang, Ye Xia, Yi-Ting Chen, Zarana Parekh, Hieu Pham, Quoc V. Le, Yunhsuan Sung, Zhen Li, Tom Duerig_

### [OpenAI] DALL-E: Zero-Shot Text-to-Image Generation [[pdf]](https://arxiv.org/abs/2102.12092)
_Aditya Ramesh, Mikhail Pavlov, Gabriel Goh, Scott Gray, Chelsea Voss, Alec Radford, Mark Chen, Ilya Sutskever_
- We created a dataset of a similar scale to JFT-300M by collecting 250 million text-images pairs from the internet
- Stage One: Learning the Visual Codebook
- Stage Two: Learning the Prior

### [OpenAI] Grokking: Generalization beyond Overfitting on Small Algorithmic Datasets [[pdf]](https://arxiv.org/pdf/2201.02177.pdf)
_Alethea Power, Yuri Burda, Harri Edwards, Igor Babuschkin, and Vedant Misra_


### [!!!] [Google Research] VideoPoet: A Large Language Model for Zero-Shot Video Generation [[pdf]](https://arxiv.org/abs/2312.14125) [[project]](https://sites.research.google/videopoet/)
_Dan Kondratyuk, Lijun Yu, Xiuye Gu, José Lezama, Jonathan Huang, Rachel Hornung, Hartwig Adam, Hassan Akbari, Yair Alon, Vighnesh Birodkar, Yong Cheng, Ming-Chang Chiu, Josh Dillon, Irfan Essa, Agrim Gupta, Meera Hahn, Anja Hauth, David Hendon, Alonso Martinez, David Minnen, David Ross, Grant Schindler, Mikhail Sirotenko, Kihyuk Sohn, Krishna Somandepalli, Huisheng Wang, Jimmy Yan, Ming-Hsuan Yang, Xuan Yang, Bryan Seybold, Lu Jiang_
- A pre-trained MAGVIT V2 video tokenizer and a SoundStream audio tokenizer transform images, video, and audio clips with variable lengths into a sequence of discrete codes in a unified vocabulary. 
- An autoregressive language model learns across video, image, audio, and text modalities to autoregressively predict the next video or audio token in the sequence.
- A mixture of multimodal generative learning objectives are introduced into the LLM training framework, including text-to-video, text-to-image, image-to-video, video frame continuation, video inpainting and outpainting, video stylization, and video-to-audio. Furthermore, such tasks can be composed together for additional zero-shot capabilities (e.g., text-to-audio).
- Datasets. We train on a total of 1B image-text pairs and ∼270M videos (∼100M with paired text, of which ∼50M are used for high-quality finetuning, and ∼170M with paired audio) from the public internet and other sources, i.e. around 2 trillion tokens across all modalities. The data has been filtered to remove egregious content and sampled to improve contextual and demographic diversity.
- ![](../assets/fig_generative_models/11.png)
- ![](../assets/fig_generative_models/12.png)

### [NeurIPS 2023] DaTaSeg: Taming a Universal Multi-Dataset Multi-Task Segmentation Model [[pdf]](https://arxiv.org/abs/2306.01736)
_Xiuye Gu, Yin Cui, Jonathan Huang, Abdullah Rashwan, Xuan Yang, Xingyi Zhou, Golnaz Ghiasi, Weicheng Kuo, Huizhong Chen, Liang-Chieh Chen, David A Ross_
- ![](../assets/fig_generative_models/15.png)

### [NeurIPS 2023] Module-wise Adaptive Distillation for Multimodality Foundation Models [[pdf]](https://arxiv.org/abs/2310.04550)
_Chen Liang, Jiahui Yu, Ming-Hsuan Yang, Matthew Brown, Yin Cui, Tuo Zhao, Boqing Gong, Tianyi Zhou_

### [NeurIPS 2023] Alternating Gradient Descent and Mixture-of-Experts for Integrated Multimodal Perception [[pdf]](https://arxiv.org/abs/2305.06324)
_Hassan Akbari, Dan Kondratyuk, Yin Cui, Rachel Hornung, Huisheng Wang, Hartwig Adam_
- IMP integrates multimodal inputs including image, video, text, and audio into a single Transformer encoder with minimal modality-specific components. IMP makes use of a novel design that **combines Alternating Gradient Descent (AGD) and Mixture-of-Experts (MoE) for efficient model & task scaling**. We conduct extensive empirical studies and reveal the following key insights: 1) performing gradient descent updates by alternating on diverse modalities, loss functions, and tasks, with varying input resolutions, efficiently improves the model. 2) sparsification with MoE on a single modalityagnostic encoder substantially improves the performance, outperforming dense models that use modality-specific encoders or additional fusion layers and greatly mitigates the conflicts between modalities.
- ![](../assets/fig_generative_models/20.png)

### [Shanghai AI Lab] InternVideo2: Scaling Video Foundation Models for Multimodal Video Understanding [[pdf]](https://arxiv.org/pdf/2403.15377.pdf) [[project]](https://github.com/OpenGVLab/InternVideo2)
_Yi Wang, Kunchang Li, Xinhao Li, Jiashuo Yu, Yinan He, Guo Chen, Baoqi Pei, Rongkun Zheng, Jilan Xu, Zun Wang, Yansong Shi, Tianxiang Jiang, Songze Li, Hongjie Zhang, Yifei Huang, Yu Qiao, Yali Wang, Limin Wang_
- explore the use of audio information in videos to improve performance
- ![](../assets/fig_generative_models/36.png)