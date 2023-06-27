# Blog Event-Based Vision

## Contents

 - [Event-based vision](#event-based-vision)
 - [Spiking Neural Networks](#spiking-neural-networks)
 - [6D Pose Estimation](#6d-pose-estimation)
 - [Optimization Human Shape Reconstruction](#optimization-human-shape-reconstruction)
 - [Video prediction and Pose transfer](#video-prediction-and-pose-transfer)
 - [Representation learning](#representation-learning)
 - [Others](#others)
 - [Transformer](#transformer)

---

## Event-based vision

### research group: [http://rpg.ifi.uzh.ch/research_dvs.html](http://rpg.ifi.uzh.ch/research_dvs.html)

### resources: [https://github.com/uzh-rpg/event-based_vision_resources](https://github.com/uzh-rpg/event-based_vision_resources)

### advantages
- Event cameras have several advantages over traditional cameras: a latency in the order of microseconds, a very high dynamic range (140 dB compared to 60 dB of traditional cameras), and very low power consumption (10mW vs 1.5W of traditional cameras). Moreover, since all pixels capture light independently, such sensors do not suffer from motion blur.

### [TPAMI 2020] Event-based Vision: A Survey [[pdf]](https://arxiv.org/abs/1904.08405)
_Guillermo Gallego, Tobi Delbruck, Garrick Orchard, Chiara Bartolozzi, Brian Taba, Andrea Censi, Stefan Leutenegger, Andrew Davison, Joerg Conradt, Kostas Daniilidis, Davide Scaramuzza_

### [CVPR 2020] EventCap: Monocular 3D Capture of High-Speed Human Motions using an Event Camera [[pdf]](https://arxiv.org/abs/1908.11505)
_Lan Xu, Weipeng Xu, Vladislav Golyanik, Marc Habermann, Lu Fang, Christian Theobalt_

### [ECCV 2020] Spike-FlowNet: Event-based Optical Flow Estimation with Energy-Efficient Hybrid Neural Networks [[pdf]](https://arxiv.org/abs/2003.06696)
_Chankyu Lee, Adarsh Kumar Kosta, Alex Zihao Zhu, Kenneth Chaney, Kostas Daniilidis, Kaushik Roy_
- SNN decodes event streams and ANN encodes optical flow. Simplest IF neuron model is used in this paper.
- Self-supervised warping loss (optical flow between neighboring frames).

### [CVPR 2020] Single Image Optical Flow Estimation With an Event Camera [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Pan_Single_Image_Optical_Flow_Estimation_With_an_Event_Camera_CVPR_2020_paper.pdf)
_Liyuan Pan, Miaomiao Liu, Richard Hartley_

### [CVPR 2018] Pwc-net: Cnns for optical flow using pyramid, warping, and cost volume [[pdf]](https://arxiv.org/abs/1709.02371) [[code]](https://github.com/NVlabs/PWC-Net)
_Deqing Sun, Xiaodong Yang, Ming-Yu Liu, Jan Kautz_

### [CVPR 2020] Learning to Super Resolve Intensity Images From Events [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/I._Learning_to_Super_Resolve_Intensity_Images_From_Events_CVPR_2020_paper.pdf)
_S. Mohammad Mostafavi I., Jonghyun Choi, Kuk-Jin Yoon_

### [CVPR 2020] Learning Event-Based Motion Deblurring [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Jiang_Learning_Event-Based_Motion_Deblurring_CVPR_2020_paper.pdf)
_Zhe Jiang, Yu Zhang, Dongqing Zou, Jimmy Ren, Jiancheng Lv, Yebin Liu_

### [CVPR 2020] Video to Events: Recycling Video Datasets for Event Cameras [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Gehrig_Video_to_Events_Recycling_Video_Datasets_for_Event_Cameras_CVPR_2020_paper.pdf)
_Daniel Gehrig, Mathias Gehrig, Javier Hidalgo-Carrio, Davide Scaramuzza_

 ### [CVPR 2020] 4D Visualization of Dynamic Events From Unconstrained Multi-View Videos [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Bansal_4D_Visualization_of_Dynamic_Events_From_Unconstrained_Multi-View_Videos_CVPR_2020_paper.pdf)
_Aayush Bansal, Minh Vo, Yaser Sheikh, Deva Ramanan, Srinivasa Narasimhan_

### [CVPR 2020] Globally Optimal Contrast Maximisation for Event-Based Motion Estimation [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Liu_Globally_Optimal_Contrast_Maximisation_for_Event-Based_Motion_Estimation_CVPR_2020_paper.pdf)
_Daqi Liu, Alvaro Parra, Tat-Jun Chin_

### [CVPR 2020] Learning Visual Motion Segmentation Using Event Surfaces [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Mitrokhin_Learning_Visual_Motion_Segmentation_Using_Event_Surfaces_CVPR_2020_paper.pdf)
_Anton Mitrokhin, Zhiyuan Hua, Cornelia Fermuller, Yiannis Aloimonos_

### [CVPR 2020] EventSR: From Asynchronous Events to Image Reconstruction, Restoration, and Super-Resolution via End-to-End Adversarial Learning [[pdf]](https://arxiv.org/pdf/2003.07640.pdf)
_Lin Wang, Tae-Kyun Kim, and Kuk-Jin Yoon_

### [ICCV 2019] Learning an event sequence embedding for dense event-based deep stereo [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Tulyakov_Learning_an_Event_Sequence_Embedding_for_Dense_Event-Based_Deep_Stereo_ICCV_2019_paper.pdf)
_Stepan Tulyakov, Francois Fleuret, Martin Kiefel, Peter Gehler, Michael Hirsch_

### [ICCV 2019] End-to-End Learning of Representations for Asynchronous Event-Based Data [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Gehrig_End-to-End_Learning_of_Representations_for_Asynchronous_Event-Based_Data_ICCV_2019_paper.pdf)
_Daniel Gehrig, Antonio Loquercio, Konstantinos G. Derpanis, Davide Scaramuzza_

### [CVPR 2019] Event-based High Dynamic Range Image and Very High Frame Rate Video Generation using Conditional Generative Adversarial Networks [[pdf]](https://arxiv.org/abs/1811.08230)
_S. Mohammad Mostafavi I., Lin Wang, Yo-Sung Ho, Kuk-Jin Yoon_

### [CVPR 2019] Unsupervised Event-Based Learning of Optical Flow, Depth, and Egomotion [[pdf]](https://arxiv.org/abs/1812.08156)
_Alex Zihao Zhu, Liangzhe Yuan, Kenneth Chaney, Kostas Daniilidis_

### [IROS 2018] Event-based Moving Object Detection and Tracking [[pdf]](https://arxiv.org/abs/1803.04523)
_Anton Mitrokhin, Cornelia Fermuller, Chethan Parameshwara, Yiannis Aloimonos_

### [CVPR 2019] Bringing a Blurry Frame Alive at High Frame-Rate With an Event Camera [[pdf]](https://arxiv.org/abs/1811.10180)
_Liyuan Pan, Cedric Scheerlinck, Xin Yu, Richard Hartley, Miaomiao Liu, Yuchao Dai_

### [CVPR 2019] Focus Is All You Need: Loss Functions For Event-based Vision [[pdf]](https://arxiv.org/abs/1904.07235)
_Guillermo Gallego, Mathias Gehrig, Davide Scaramuzza_

### [CVPR 2019] Event Cameras, Contrast Maximization and Reward Functions: An Analysis [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Stoffregen_Event_Cameras_Contrast_Maximization_and_Reward_Functions_An_Analysis_CVPR_2019_paper.pdf)
_Timo Stoffregen, Lindsay Kleeman_

### [TPAMI 2018] Event-based, 6-DOF Camera Tracking from Photometric Depth Maps [[pdf]](http://rpg.ifi.uzh.ch/docs/PAMI17_Gallego.pdf)
_Guillermo Gallego, Jon E.A. Lund, Elias Mueggler, Henri Rebecq, Tobi Delbruck, Davide Scaramuzza_

### [IJCV 2017, BMVC 2016] EMVS: Event-based Multi-View Stereo - 3D Reconstruction with an Event Camera in Real-Time [[pdf]](https://supitalp.github.io/research/publication/emvs_ijcv/)
_Henri Rebecq, Guillermo Gallego, Elias Mueggler, Davide Scaramuzza_

### [ECCV 2018] Asynchronous, Photometric Feature Tracking using Events and Frames [[pdf]](https://arxiv.org/abs/1807.09713)
_Daniel Gehrig, Henri Rebecq, Guillermo Gallego, Davide Scaramuzza_

### [CVPR 2018] A Unifying Contrast Maximization Framework for Event Cameras, with Applications to Motion, Depth and Optical Flow Estimation [[pdf]](https://arxiv.org/abs/1804.01306)
_Guillermo Gallego, Henri Rebecq, Davide Scaramuzza_
- We present a unifying framework to solve several computer vision problems with event cameras: motion, depth and optical flow estimation. The main idea of our framework is to find the point trajectories on the image plane that are best aligned with the event data by maximizing an objective function: the contrast of an image of warped events. Our method implicitly handles data association between the events, and therefore, does not rely on additional appearance information about the scene. In addition to accurately recovering the motion parameters of the problem, our framework produces motion-corrected edge-like images with high dynamic range that can be used for further scene analysis.

### [ECCV 2018] Semi-Dense 3D Reconstruction with a Stereo Event Camera [[pdf]](https://arxiv.org/abs/1807.07429)
_Yi Zhou, Guillermo Gallego, Henri Rebecq, Laurent Kneip, Hongdong Li, Davide Scaramuzza_

### [CVPR 2019, TPAMI 2020] Events-to-Video: Bringing Modern Computer Vision to Event Cameras [[pdf]](https://arxiv.org/abs/1904.08298) [[pdf]](https://arxiv.org/pdf/1906.07165.pdf)
_Henri Rebecq, René Ranftl, Vladlen Koltun, Davide Scaramuzza_
- Since **the output of event cameras is fundamentally different from conventional cameras**, it is commonly accepted that they require the development of specialized algorithms to accommodate the particular nature of events.
- We propose a novel recurrent network to reconstruct videos from a stream of events, and train it on a large amount of simulated event data.

### [ECCV 2018 workshop] Unsupervised event-based optical flow using motion compensation [[pdf]](https://arxiv.org/abs/1812.08156)
_Alex Zihao Zhu, Liangzhe Yuan, Kenneth Chaney, Kostas Daniilidis_

### [Scientific Report] A Spiking Neural Network Model of Depth from Defocus for Event-based Neuromorphic Vision [[pdf]](https://www.nature.com/articles/s41598-019-40064-0.pdf)
_Germain Haessig, Xavier Berthelon, Sio-Hoi Ieng & Ryad Benosman_

### [CVPR 2017] A Low Power, Fully Event-Based Gesture Recognition System [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Amir_A_Low_Power_CVPR_2017_paper.pdf) [[dataset]](http://research.ibm.com/dvsgesture/)
_Arnon Amir, Brian Taba, David Berg, Timothy Melano, Jeffrey McKinstry, Carmelo Di Nolfo, Tapan Nayak, Alexander Andreopoulos, Guillaume Garreau, Marcela Mendoza, Jeff Kusnitz, Michael Debole, Steve Esser, Tobi Delbruck, Myron Flickner, and Dharmendra Modha_

### [CVPR 2019] EV-Gait: Event-Based Robust Gait Recognition Using Dynamic Vision Sensors [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Wang_EV-Gait_Event-Based_Robust_Gait_Recognition_Using_Dynamic_Vision_Sensors_CVPR_2019_paper.pdf)
_Yanxiang Wang, Bowen Du, Yiran Shen, Kai Wu, Guangrong Zhao, Jianguo Sun, Hongkai Wen_

### [CVPR workshop 2019] DHP19: Dynamic Vision Sensor 3D Human Pose Dataset [[pdf]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/EventVision/Calabrese_DHP19_Dynamic_Vision_Sensor_3D_Human_Pose_Dataset_CVPRW_2019_paper.pdf)
_Enrico Calabrese, Gemma Taverni, Christopher Awai Easthope, Sophie Skriabine, Federico Corradi, Luca Longinotti, Kynan Eng, Tobi Delbruck_

### [RoSS 2018] EV-FlowNet: Self-supervised optical flow estimation for event-based cameras [[pdf]](https://arxiv.org/abs/1802.06898)
_Alex Zihao Zhu, Liangzhe Yuan, Kenneth Chaney, Kostas Daniilidis_
- In particular, we introduce an image based representation of a given event stream, which is fed into a self-supervised neural network as the sole input. The corresponding grayscale images captured from the same camera at the same time as the events are then used as a supervisory signal to provide a loss function at training time, given the estimated flow from the network.

### [CVPR 2016] Simultaneous Optical Flow and Intensity Estimation from an Event Camera [[pdf]](https://openaccess.thecvf.com/content_cvpr_2016/papers/Bardow_Simultaneous_Optical_Flow_CVPR_2016_paper.pdf)
_Patrick Bardow, Andrew J. Davison, Stefan Leutenegger_


### [NNLS 2014] Event-Based Visual Flow [[pdf]](https://ieeexplore.ieee.org/document/6589170) [[code]](https://github.com/winswang/event-flow)
_Ryad Benosman, Charles Clercq, Xavier Lagorce, Sio-Hoi Ieng, and Chiara Bartolozzi_


[[back to top]](#contents)

---

## Spiking Neural Networks

### [NeurIPS 2022] Online Training Through Time for Spiking Neural Networks [[pdf]](https://arxiv.org/pdf/2210.04195.pdf)
_Mingqing Xiao, Qingyan Meng, Zongpeng Zhang, Di He, Zhouchen Lin_

### [NeurIPS 2022] Toward Robust Spiking Neural Network Against Adversarial Perturbation [[pdf]](https://arxiv.org/abs/2205.01625)
_Ling Liang, Kaidi Xu, Xing Hu, Lei Deng, Yuan Xie_

### [NeurIPS 2022] Training Spiking Neural Networks with Local Tandem Learning [[pdf]](https://arxiv.org/abs/2210.04532)
_Qu Yang, Jibin Wu, Malu Zhang, Yansong Chua, Xinchao Wang, Haizhou Li_

### [NeurIPS 2022] GLIF: A Unified Gated Leaky Integrate-and-Fire Neuron for Spiking Neural Networks [[pdf]](https://arxiv.org/abs/2210.13768)
_Xingting Yao, Fanrong Li, Zitao Mo, Jian Cheng_


### [ICLR 2022] Temporal Efficient Training of Spiking Neural Network via Gradient Re-weighting [[pdf]](https://arxiv.org/abs/2202.11946)
_Shikuang Deng, Yuhang Li, Shanghang Zhang, Shi Gu_

### [CVPR 2022] Event Transformer. A sparse-aware solution for efficient event data processing [[pdf]](https://arxiv.org/abs/2204.03355)
_Alberto Sabater, Luis Montesano, Ana C. Murillo_
- Event cameras are sensors of great interest for many applications that run in low-resource and challenging environments. They log sparse illumination changes with high temporal resolution and high dynamic range, while they present minimal power consumption. However, top-performing methods often ignore specific event-data properties, leading to the development of generic but computationally expensive algorithms. Efforts toward efficient solutions usually do not achieve top-accuracy results for complex tasks. This work proposes a novel framework, Event Transformer (EvT), that effectively takes advantage of event-data properties to be highly efficient and accurate. We introduce a new patch-based event representation and a compact transformer-like architecture to process it. EvT is evaluated on different event-based benchmarks for action and gesture recognition. Evaluation results show better or comparable accuracy to the state-of-the-art while requiring significantly less computation resources, which makes EvT able to work with minimal latency both on GPU and CPU.

### [CVPR 2022] Spiking Transformers for Event-based Single Object Tracking [[pdf]](https://zhangjiqing.com/publication/stnet/)
_Jiqing Zhang, Bo Dong, Haiwei Zhang, Jianchuan Ding, Felix Heide, Baocai Yin, Xin Yang_
- Event-based cameras bring a unique capability to tracking, being able to function in challenging real-world conditions as a direct result of their high temporal resolution and high dynamic range.  These imagers capture events asynchronously that encode rich temporal and spatial information. However, effectively extracting this information from events remains an open challenge. In this work, we propose a spiking transformer network, STNet, for single object tracking. STNet dynamically extracts and fuses information from both temporal and spatial domains. In particular, the proposed architecture features a transformer module to provide global spatial information and a spiking neural network (SNN) module for extracting temporal cues. The spiking threshold of the SNN module is dynamically adjusted based on the statistical cues of the spatial information, which we find essential in providing robust SNN features. We fuse both feature branches dynamically with a novel cross-domain attention fusion algorithm. Extensive experiments on two event-based datasets, FE240hz and EED, validate that the proposed STNet outperforms existing state-of-the-art methods in both tracking accuracy and speed with a significant margin.
- The proposed SFE relies on a 3-layer LIF-based SNN [45] and a reduced Swin-transformer [33] to capture informative cues from the temporal and spatial domains.

### [Neurips 2021] Deep Residual Learning in Spiking Neural Networks [[pdf]](https://arxiv.org/abs/2102.04159)
_Wei Fang, Zhaofei Yu, Yanqi Chen, Tiejun Huang, Timothée Masquelier, Yonghong Tian_
- In this paper, we propose the spike element-wise (SEW) ResNet to realize residual learning in deep SNNs. We prove that the SEW ResNet can easily implement identity mapping and overcome the vanishing/exploding gradient problems of Spiking ResNet.

### [ICCV 2019] Incorporating Learnable Membrane Time Constant to Enhance Learning of Spiking Neural Networks [[pdf]](https://arxiv.org/abs/2007.05785)
_Wei Fang, Zhaofei Yu, Yanqi Chen, Timothee Masquelier, Tiejun Huang, Yonghong Tian_

### [Neurips 2021] Differentiable Spike: Rethinking Gradient-Descent for Training Spiking Neural Networks [[pdf]](https://proceedings.neurips.cc/paper/2021/file/c4ca4238a0b923820dcc509a6f75849b-Paper.pdf)
_Yuhang Li, Yufei Guo, Shanghang Zhang, Shikuang Deng, Yongqing Hai, Shi Gu_

### [Neurips 2021] Training Feedback Spiking Neural Networks by Implicit Differentiation on the Equilibrium State [[pdf]](https://arxiv.org/pdf/2109.14247.pdf)
_Mingqing Xiao, Qingyan Meng, Zongpeng Zhang, Yisen Wang, Zhouchen Lin_

### [Neurips 2020] Unifying Activation- and Timing-based Learning Rules for Spiking Neural Networks [[pdf]](https://arxiv.org/abs/2006.02642)
_Jinseok Kim, Kyungsu Kim, Jae-Joon Kim_

### [Neurips 2020] Temporal Spike Sequence Learning via Backpropagation for Deep Spiking Neural Networks [[pdf]](https://arxiv.org/abs/2002.10085)
_Wenrui Zhang, Peng Li_
- We present a novel Temporal Spike Sequence Learning Backpropagation (TSSL-BP) method for training deep SNNs, 
null- which breaks down error backpropagation across two types of inter-neuron and intra-neuron dependencies 
null- and leads to improved temporal learning precision.
- Wulfram Gerstner and Werner M Kistler. Spiking neuron models: Single neurons, populations, plasticity. 
null- Cambridge university press, 2002.

### [Neurips 2021] Self-Supervised Learning of Event-Based Optical Flow with Spiking Neural Networks [[pdf]](https://arxiv.org/abs/2106.01862)[[code]](https://github.com/tudelft/event_flow)
_Jesse Hagenaars, Federico Paredes-Vallés, Guido de Croon_

### [Neurips 2021] Sparse Spiking Gradient Descent [[pdf]](https://arxiv.org/abs/2105.08810) [[code]](https://github.com/npvoid/SparseSpikingBackprop)
_Nicolas Perez-Nieves, Dan F.M. Goodman_
- Emre O. Neftci, Hesham Mostafa, and Friedemann Zenke. Surrogate gradient learning in 
null- spiking neural networks: Bringing the power of gradient-based optimization to spiking neural 
null- networks. IEEE Signal Processing Magazine, 36(6):51–63, 2019.
- Friedemann Zenke and Tim P Vogels. The remarkable robustness of surrogate gradient learning 
null- for instilling complex function in spiking neural networks. Neural Computation, 33(4):899–925, 2021.

### [CVPR 2021] Temporal-wise Attention Spiking Neural Networks for Event Streams Classification [[pdf]](https://arxiv.org/abs/2107.11711)
_Man Yao, Huanhuan Gao, Guangshe Zhao, Dingheng Wang, Yihan Lin, Zhaoxu Yang, Guoqi Li_
- Yin Bi, Aaron Chadha, Alhabib Abbas, Eirina Bourtsoulatze, and Yiannis Andreopoulos. Graph-based spatio-temporal 
null- feature learning for neuromorphic vision sensing. IEEE Transactions on Image Processing, 29:9084–9098, 2020.
- Kaushik Roy, Akhilesh Jaiswal, and Priyadarshini Panda. Towards spike-based machine intelligence with neuromorphic 
null- computing. Nature, 575(7784):607–617, 2019.
- Zhenzhi Wu, Hehui Zhang, Yihan Lin, Guoqi Li, Meng Wang, and Ye Tang. Liaf-net: Leaky integrate and analog fire 
null- network for lightweight and efficient spatiotemporal information processing. IEEE Transactions on Neural Networks 
null- and Learning Systems, pages 1–14, 2021.
- Jie Hu, Li Shen, and Gang Sun. Squeeze-and-excitation networks. In Proceedings of the IEEE conference on computer 
null- vision and pattern recognition, pages 7132–7141, 2018.
- We use the STBP [38] and the BPTT algorithm [40] to train LIF-SNNs and LIAFSNNs, respectively.

### [Neurips 2018] Gradient Descent for Spiking Neural Networks [[pdf]](https://papers.nips.cc/paper/2018/file/185e65bc40581880c4f2c82958de8cfe-Paper.pdf)
_Dongsung Huh, Terrence J. Sejnowski_
- In general, the exact gradient of a dynamical system can be calculated using either Pontryagin’s minimum principle [33], also known as backpropagation through time, or real-time recurrent learning, which yield identical results.

### [ECCV 2020] Spike-FlowNet: Event-based Optical Flow Estimation with Energy-Efficient Hybrid Neural Networks [[pdf]](https://arxiv.org/abs/2003.06696)
_Chankyu Lee, Adarsh Kumar Kosta, Alex Zihao Zhu, Kenneth Chaney, Kostas Daniilidis, Kaushik Roy_
- SNN decodes event streams and ANN encodes optical flow. Simplest IF neuron model is used in this paper.
- Self-supervised warping loss (optical flow between neighboring frames).

### [ArXiv 2018] Deep Learning in Spiking Neural Networks [[pdf]](https://arxiv.org/pdf/1804.08150.pdf)
_Amirhossein Tavanaei, Masoud Ghodrati, Saeed Reza Kheradpisheh, Timothee Masquelier, Anthony S. Maida_
- Fully Connected SNNs
- Spiking CNN [173] [57][165][183]
- ANN-to-SNN conversion

### [IROS 2022] SpikeMS: Deep Spiking Neural Network for Motion Segmentation [[pdf]](https://arxiv.org/abs/2105.06562)
_Chethan M. Parameshwara, Simin Li, Cornelia Fermüller, Nitin J. Sanket, Matthew S. Evanusa, Yiannis Aloimonos_

### [TPAMI 2019] Unsupervised Learning of a Hierarchical Spiking Neural Network for Optical Flow Estimation: From Events to Global Motion Perception [[pdf]](https://arxiv.org/abs/1807.10936)
_Federico Paredes-Vallés, Kirk Y. W. Scheper, Guido C. H. E. de Croon_

### [Frontier in Neuroscience 2020] Enabling Spike-Based Backpropagation for Training Deep Neural Network Architectures [[pdf]](https://arxiv.org/abs/1903.06379)
_Chankyu Lee, Syed Shakib Sarwar, Priyadarshini Panda, Gopalakrishnan Srinivasan, Kaushik Roy_

### [Frontier in Neuroscience 2020] Toward Scalable, Efficient, and Accurate Deep Spiking Neural Networks With Backward Residual Connections, Stochastic Softmax, and Hybridization [[pdf]](https://arxiv.org/abs/1910.13931)
_Priyadarshini Panda, Aparna Aketi, Kaushik Roy_

### [Frontier in Neuroscience 2018] Spatio-temporal backpropagation for training high-performance spiking neural networks [[pdf]](https://arxiv.org/abs/1706.02609)
_Yujie Wu, Lei Deng, Guoqi Li, Jun Zhu, Luping Shi_

### [arXiv 2019] Surrogate Gradient Learning in Spiking Neural Networks [[pdf]](https://arxiv.org/abs/1901.09948)
_Emre O. Neftci, Hesham Mostafa, Friedemann Zenke_

### [ICLR 2018] Deep rewiring: Training very sparse deep networks [[pd]](https://arxiv.org/abs/1711.05136)
_Guillaume Bellec, David Kappel, Wolfgang Maass, Robert Legenstein_

### [NeurIPS 2018] Long short-term memory and learning-to-learn in networks of spiking neurons [[pdf]](https://arxiv.org/abs/1803.09574)
_Guillaume Bellec, Darjan Salaj, Anand Subramoney, Robert Legenstein, Wolfgang Maass_

### [NeurIPS 2018] Slayer: Spike layer error reassignment in time [[pdf]](https://arxiv.org/abs/1810.08646)
_Sumit Bam Shrestha, Garrick Orchard_

### Time structure of the activity in neural network models [[pdf]](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.51.738)
_Wulfram Gerstner_
- Spiking Response Model used in Slayer

### [ICRA 2015] Spike time based unsupervised learning of receptive fields for event-driven vision [[pdf]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7139786&tag=1)
_Himanshu Akolkar, Stefano Panzeri and Chiara Bartolozzi_


### Convolutional networks for fast, energy-efficient neuromorphic computing [[pdf]](https://arxiv.org/pdf/1603.08270.pdf)
_Steven K. Esser, Paul A. Merolla, John V. Arthur, Andrew S. Cassidy, Rathinakumar Appuswamy, Alexander Andreopoulos, David J. Berg, Jeffrey L. McKinstry, Timothy Melano, Davis R. Barch, Carmelo di Nolfo, Pallab Datta, Arnon Amir, Brian Taba, Myron D. Flickner, and Dharmendra S. Modha._

### A wafer-scale neuromorphic hardware system for large-scale neural modeling [[pdf]](https://ieeexplore.ieee.org/document/5536970)
_Johannes Schemmel, Daniel Br¨uderle, Andreas Gr¨ubl, Matthias Hock, Karlheinz Meier, and Sebastian Millner_

### [IEEE NNLS 2018] A supervised learning algorithm for learning precise timing of multiple spikes in multilayer spiking neural networks [[pdf]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8305661)
_Aboozar Taherkhani, Ammar Belatreche, Yuhua Li, Liam P. Maguire_

### [Frontier in Neuroscience 2017] Conversion of continuous-valued deep networks to efficient eventdriven networks for image classification [[pdf]](https://www.frontiersin.org/articles/10.3389/fnins.2017.00682/full)
_Bodo Rueckauer, Iulia-Alexandra Lungu, Yuhuang Hu, Michael Pfeiffer and Shih-Chii Liu_

### [Frontier in Neuroscience 2016] Training Deep Spiking Neural Networks using Backpropagation [[pdf]](https://arxiv.org/abs/1608.08782)
_Jun Haeng Lee, Tobi Delbruck, Michael Pfeiffer_

### [Annual Review of Neuroscience 2008] Spike Timing–Dependent Plasticity: A Hebbian Learning Rule [[pdf]](https://www.annualreviews.org/doi/pdf/10.1146/annurev.neuro.31.060407.125639)
_Natalia Caporale and Yang Dan_



[[back to top]](#contents)

---

## 6D Pose Estimation

### [CVPR 2020] Learning deep network for detecting 3D object keypoints and 6D poses [[pdf]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhao_Learning_Deep_Network_for_Detecting_3D_Object_Keypoints_and_6D_CVPR_2020_paper.pdf)
_Wanqing Zhao, Shaobo Zhang, Ziyu Guan, Wei Zhao_

### [CVPR 2019] Pvnet: Pixel-wise voting network for 6dof pose estimation [[pdf]](https://arxiv.org/abs/1812.11788.pdf)[[code]](https://zju3dv.github.io/pvnet/)
_Sida Peng, Yuan Liu, Qixing Huang, Hujun Bao, Xiaowei Zhou_

### [CVPR 2020] Pvn3d: A deep point-wise 3d keypointsvoting network for 6dof pose estimation [[pdf]](https://arxiv.org/abs/1911.04231.pdf)
_Yisheng He, Wei Sun, Haibin Huang, Jianran Liu, Haoqiang Fan, Jian Sun_

### [ICCV 2019] Pix2pose: Pixel-wise coordinate regression of objects for 6d pose estimation [[pdf]](https://arxiv.org/abs/1908.07433.pdf)
_Kiru Park, Timothy Patten, Markus Vincze_

### [CVPR 2018] Real-time seamless single shot 6d object pose prediction [[pdf]](https://arxiv.org/abs/1711.08848)
_Bugra Tekin, Sudipta N. Sinha, Pascal Fua_

### [ECCV 2018] DeepIM: Deep iterative matching for 6d pose estimation [[pdf]](https://arxiv.org/abs/1804.00175.pdf)
_Yi Li, Gu Wang, Xiangyang Ji, Yu Xiang, Dieter Fox_

### [ECCV 2018 Best Paper Award] Implicit 3D Orientation Learning for 6D Object Detection from RGB Images [[pdf]](https://arxiv.org/abs/1902.01275.pdf)
_Martin Sundermeyer, Zoltan-Csaba Marton, Maximilian Durner, Manuel Brucker, Rudolph Triebel_

### [ICRA 2017] 6-dof object pose from semantic keypoints [[pdf]](https://arxiv.org/abs/1703.04670)
_Georgios Pavlakos, Xiaowei Zhou, Aaron Chan, Konstantinos G. Derpanis, Kostas Daniilidis_

### [ICCV 2017] BB8: A Scalable, Accurate, Robust to Partial Occlusion Method for Predicting the 3D Poses of Challenging Objects without Using Depth [[pdf]](https://arxiv.org/pdf/1703.10896.pdf)
_Mahdi Rad, Vincent Lepetit_


[[back to top]](#contents)

---

## Optimization Human Shape Reconstruction


### Background studying 1
- quaternion \\((w, x, y, z))\\) 
	- [[good tutorial]](https://www.zhihu.com/question/23005815)
	- [[Accurate Computation of Quaternions from Rotation Matrices]](http://www.iri.upc.edu/files/scidoc/2068-Accurate-Computation-of-Quaternions-from-Rotation-Matrices.pdf)
	- [[Rodrigues vector to rotation matrix]](https://www2.cs.duke.edu/courses/fall13/compsci527/notes/rodrigues.pdf) [[wiki]](https://en.wikipedia.org/wiki/Rodrigues%27_rotation_formula)


### Background studying 2
- TSDF [[reference]](https://blog.csdn.net/qq_39732684/article/details/105294993)
 ![2020-polarization-clothed-human-shape](./attachments/2020-polarization-clothed-human-shape.md)

### [CVPR 2018] DoubleFusion: Real-time Capture of Human Performances with Inner Body Shapes from a Single Depth Sensor [[pdf]](https://arxiv.org/abs/1804.06023)
_Tao Yu, Zerong Zheng, Kaiwen Guo, Jianhui Zhao, Qionghai Dai, Hao Li, Gerard Pons-Moll, Yebin Liu_

### [CVPR 2015]  Dynamicfusion: Reconstruction and tracking of non-rigid scenes in real-time [[pdf]](https://grail.cs.washington.edu/projects/dynamicfusion/papers/DynamicFusion.pdf)
_Richard Newcombe, Dieter Fox, Steve Seitz_
- [[reference]](https://blog.csdn.net/fuguangping/article/details/105766665)

### [ToG 2017] Real-time geometry, albedo and motion reconstruction using a single rgbd camera [[pdf]](https://www.guokaiwen.com/main.pdf)
_K. Guo, F. Xu, T. Yu, X. Liu, Q. Dai, and Y. Liu_

### [ICCV 2017] Bodyfusion: Real-time capture of human motion and surface geometry using a single depth camera [[pdf]](https://openaccess.thecvf.com/content_ICCV_2017/papers/Yu_BodyFusion_Real-Time_Capture_ICCV_2017_paper.pdf)
_T. Yu, K. Guo, F. Xu, Y. Dong, Z. Su, J. Zhao, J. Li, Q. Dai, and Y. Liu_

### [ECCV 2016] Volumedeform: Real-time volumetric nonrigid reconstruction [[pdf]](https://graphics.stanford.edu/~niessner/papers/2016/5volumeDeform/innmann2016deform.pdf)
_M. Innmann, M. Zollhofer, M. Nießner, C. Theobalt, and M. Stamminger._

### [ECCV 2018] ArticulatedFusion: Real-time Reconstruction of Motion, Geometry and Segmentation Using a Single Depth Camera [[pdf]](https://openaccess.thecvf.com/content_ECCV_2018/papers/Chao_Li_ArticulatedFusion_Real-time_Reconstruction_ECCV_2018_paper.pdf)
_Chao Li, Zheheng Zhao, and Xiaohu Guo_

### [CVPR 2014, TPAMI 2016] Real-Time Simultaneous Pose and Shape Estimation for Articulated Objects Using a Single Depth Camera [[pdf]](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.663.8898&rep=rep1&type=pdf) [[pdf]](https://ieeexplore.ieee.org/document/7457693)
_Mao Ye, Yang Shen, Chao Du, Zhigeng Pan, Ruigang Yang_


[[back to top]](#contents)

---

## Video Prediction and Pose Transfer

### [NeurIPS 2016] Generating Videos with Scene Dynamics [[pdf]](https://arxiv.org/abs/1609.02612)
_Carl Vondrick, Hamed Pirsiavash, Antonio Torralba_
- ![](../assets/fig_research_diary/4.PNG)

### [ICLR 2016] Deep multi-scale video prediction beyond mean square error [[pdf]](https://arxiv.org/abs/1511.05440)
_Michael Mathieu, Camille Couprie, Yann LeCun_

### [ICCV 2017] The Pose Knows: Video Forecasting by Generating Pose Futures [[pdf]](https://arxiv.org/abs/1705.00053)
_Jacob Walker, Kenneth Marino, Abhinav Gupta, Martial Hebert_
- ![](../assets/fig_research_diary/5.PNG)

### [ECCV 2018] Deep Video Generation, Prediction and Completion of Human Action Sequences [[pdf]](https://arxiv.org/abs/1711.08682)
_Haoye Cai, Chunyan Bai, Yu-Wing Tai, Chi-Keung Tang_
- ![](../assets/fig_research_diary/6.PNG)

### [ECCV 2018] Pose Guided Human Video Generation [[PDF]](https://arxiv.org/abs/1807.11152)
_Ceyuan Yang, Zhe Wang, Xinge Zhu, Chen Huang, Jianping Shi, Dahua Lin_
- ![](../assets/fig_research_diary/7.PNG)

### [NeurIPS 2018] Video Prediction via Selective Sampling [[pdf]](https://papers.nips.cc/paper/7442-video-prediction-via-selective-sampling.pdf)
_Jingwei Xu, Bingbing Ni, Xiaokang Yang_

### [ICML 2018] Stochastic Video Generation with a Learned Prior [[pdf]](https://arxiv.org/abs/1802.07687)
_Emily Denton, Rob Fergus_

### [ICLR 2018] Stochastic Variational Video Prediction [[pdf]](https://arxiv.org/abs/1710.11252)
_Mohammad Babaeizadeh, Chelsea Finn, Dumitru Erhan, Roy H. Campbell, Sergey Levine_

### [CVPR 2019] Learning to Film from Professional Human Motion Videos [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Huang_Learning_to_Film_From_Professional_Human_Motion_Videos_CVPR_2019_paper.pdf)
_Chong Huang, Chuan-En Lin, Zhenyu Yang, Yan Kong, Peng Chen, Xin Yang, Kwang-Ting Cheng_

### [ICCV 2019] Improved Conditional VRNNs for Video Prediction [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Castrejon_Improved_Conditional_VRNNs_for_Video_Prediction_ICCV_2019_paper.pdf)
_Lluis Castrejon, Nicolas Ballas, Aaron Courville_

### [ICCV 2019] Compositional Video Prediction [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Ye_Compositional_Video_Prediction_ICCV_2019_paper.pdf)
_Yufei Ye, Maneesh Singh, Abhinav Gupta, Shubham Tulsiani_

### [NeurIPS 2019] High Fidelity Video Prediction with Large Stochastic Recurrent Neural Networks [[pdf]](https://arxiv.org/abs/1911.01655)
_Ruben Villegas, Arkanath Pathak, Harini Kannan, Dumitru Erhan, Quoc V. Le, Honglak Lee_

### [ICML 2018] Hierarchical Long-term Video Prediction without Supervision [[pdf]](https://arxiv.org/abs/1806.04768)
_Nevan Wichers, Ruben Villegas, Dumitru Erhan, Honglak Lee_
- visual analogy network (VAN), Deep visual analogy-making, NeurIPS 2015

### [ICML 2017] Learning to Generate Long-term Future via Hierarchical Prediction [[pdf]](https://arxiv.org/abs/1704.05831)
_Ruben Villegas, Jimei Yang, Yuliang Zou, Sungryull Sohn, Xunyu Lin, Honglak Lee_
- ![](../assets/fig_research_diary/10.png)

### [ECCV 2018] Flow-Grounded Spatial-Temporal Video Prediction from Still Images [[pdf]](https://arxiv.org/abs/1807.09755)
_Yijun Li, Chen Fang, Jimei Yang, Zhaowen Wang, Xin Lu, Ming-Hsuan Yang_

### [ICML 2020] Stochastic Latent Residual Video Prediction [[pdf]](https://arxiv.org/pdf/2002.09219)
_Jean-Yves Franceschi, Edouard Delasalles, Mickaël Chen, Sylvain Lamprier, Patrick Gallinari_

### [CVPR 2020] Exploring Spatial-Temporal Multi-Frequency Analysis for High-Fidelity and Temporal-Consistency Video Prediction [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Jin_Exploring_Spatial-Temporal_Multi-Frequency_Analysis_for_High-Fidelity_and_Temporal-Consistency_Video_Prediction_CVPR_2020_paper.pdf)
_Beibei Jin, Yu Hu, Qiankun Tang, Jingyu Niu, Zhiping Shi, Yinhe Han, Xiaowei Li_

### [CVPR 2020] G3AN: Disentangling Appearance and Motion for Video Generation [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Wang_G3AN_Disentangling_Appearance_and_Motion_for_Video_Generation_CVPR_2020_paper.pdf)
_Yaohui Wang, Piotr Bilinski, Francois Bremond, Antitza Dantcheva_

### [CVPR 2020] Future Video Synthesis With Object Motion Prediction [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Wu_Future_Video_Synthesis_With_Object_Motion_Prediction_CVPR_2020_paper.pdf)
_Yue Wu, Rongrong Gao, Jaesik Park, Qifeng Chen_

### [CVPR 2020] Non-Adversarial Video Synthesis With Learned Priors [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Aich_Non-Adversarial_Video_Synthesis_With_Learned_Priors_CVPR_2020_paper.pdf)
_Abhishek Aich, Akash Gupta, Rameswar Panda, Rakib Hyder, M. Salman Asif, Amit K. Roy-Chowdhury_

### [CVPR 2020] Probabilistic Video Prediction From Noisy Data With a Posterior Confidence [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Wang_Probabilistic_Video_Prediction_From_Noisy_Data_With_a_Posterior_Confidence_CVPR_2020_paper.pdf)
_Yunbo Wang, Jiajun Wu, Mingsheng Long, Joshua B. Tenenbaum_

### [CVPR 2020] Disentangling Physical Dynamics From Unknown Factors for Unsupervised Video Prediction [[pdf]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Le_Guen_Disentangling_Physical_Dynamics_From_Unknown_Factors_for_Unsupervised_Video_Prediction_CVPR_2020_paper.pdf)
_Vincent Le Guen, Nicolas Thome_

### Pose Transfer

### [NeurIPS 2019] Unsupervised Keypoint Learning for Guiding Class-Conditional Video Prediction [[pdf]](https://papers.nips.cc/paper/8637-unsupervised-keypoint-learning-for-guiding-class-conditional-video-prediction.pdf)
_Yunji Kim, Seonghyeon Nam, In Cho, and Seon Joo Kim_
- ![](../assets/fig_research_diary/8.PNG)
- [NeurIPS 2018] Unsupervised learning of object landmarks through conditional image generation [[pdf]](https://arxiv.org/abs/1806.07823)
- ![](../assets/fig_research_diary/9.png)

### [ICCV 2019] Everybody Dance Now [[pdf]](https://arxiv.org/abs/1808.07371)
_Caroline Chan, Shiry Ginosar, Tinghui Zhou, Alexei A. Efros_
- ![](../assets/fig_research_diary/12.PNG)

### [CVPR 2018] Synthesizing Images of Humans in Unseen Poses [[pdf]](https://arxiv.org/abs/1804.07739)
_Guha Balakrishnan, Amy Zhao, Adrian V. Dalca, Fredo Durand, John Guttag_
- ![](../assets/fig_research_diary/13.PNG)

### [CVPR 2019] Animating Arbitrary Objects via Deep Motion Transfer [[pdf]](https://arxiv.org/abs/1812.08861)
_Aliaksandr Siarohin, Stéphane Lathuilière, Sergey Tulyakov, Elisa Ricci, Nicu Sebe_
- ![](../assets/fig_research_diary/14.PNG)

### [NeurIPS 2019] Few-shot Video-to-Video Synthesis [[pdf]](https://papers.nips.cc/paper/8746-few-shot-video-to-video-synthesis.pdf)
_Ting-Chun Wang, Ming-Yu Liu, Andrew Tao, Guilin Liu, Jan Kautz, Bryan Catanzaro_

### [CVPR 2019] Dense Intrinsic Appearance Flow for Human Pose Transfer [[pdf]](https://arxiv.org/abs/1903.11326)
_Yining Li, Chen Huang, Chen Change Loy_
- ![](../assets/fig_research_diary/15.PNG)

### [ICCV 2019] Liquid Warping GAN: A Unified Framework for Human Motion Imitation, Appearance Transfer and Novel View Synthesis [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_Liquid_Warping_GAN_A_Unified_Framework_for_Human_Motion_Imitation_ICCV_2019_paper.pdf)
_Wen Liu, Zhixin Piao, Jie Min, Wenhan Luo, Lin Ma, Shenghua Gao_
- ![](../assets/fig_research_diary/16.PNG)
- The first body mesh recovery module will estimate the 3D mesh of \\\(I_s\\\) and \\\(I_r\\\), and render their correspondence maps, \\\(C_s\\\) and \\\(C_t\\\).
- We calculate the transformation flow \\(T \in \mathbb{R}^{H×W×2}\\) by matching the correspondences between source correspondence map with its mesh face coordinates \\(f_s\\) and reference correspondence map. Here \\(H×W\\) is the size of image. Consequently, a front image \\(I_{ft}\\) and a masked background image \\(I_{bg}\\) are derived from masking the source image \\(I_s\\) based on \\(C_s\\). Finally, we warp the source image \\(I_s\\) by the transformation flow \\(T\\), and obtain the warped image \\(I_{syn}\\).
- Correspondences: Each pixel of an IUV image refers to a body part index \\(I\\), and \\((U, V)\\) coordinates that map to a unique point on the body model surface.

### [CVPR 2018] Unsupervised person image synthesis in arbitrary poses [[pdf]](https://arxiv.org/abs/1809.10280)
_Albert Pumarola, Antonio Agudo, Alberto Sanfeliu, Francesc Moreno-Noguer_
- ![](../assets/fig_research_diary/17.PNG)

### [ECCV 2018] Dense pose transfer [[pdf]](https://arxiv.org/abs/1809.01995)
_Natalia Neverova, Rıza Alp G¨uler, and Iasonas Kokkinos_
- ![](../assets/fig_research_diary/18.PNG)

### [NeurIPS 2017] Pose guided person image generation [[pdf]](https://arxiv.org/abs/1705.09368)
_Liqian Ma, Xu Jia, Qianru Sun, Bernt Schiele, Tinne Tuytelaars and Luc Van Gool_
- ![](../assets/fig_research_diary/19.PNG)

### [CVPR 2018] A variational u-net for conditional appearance and shape generation [[pdf]](https://arxiv.org/abs/1804.04694)
_Patrick Esser, Ekaterina Sutter, and Bj¨orn Ommer_
- ![](../assets/fig_research_diary/20.PNG)

### [CVPR 2018] Deformable gans for pose-based human image generation [[pdf]](https://arxiv.org/abs/1801.00055)
_Aliaksandr Siarohin, Enver Sangineto, Stphane Lathuilire, and Nicu Sebe_
- ![](../assets/fig_research_diary/21.PNG)

### [NeurIPS 2018]  Soft-gated warping-gan for pose-guided person image synthesis [[pdf]](https://arxiv.org/abs/1810.11610)
_Haoye Dong, Xiaodan Liang, Ke Gong, Hanjiang Lai, Jia Zhu, and Jian Yin_

### [NeurIPS 2015] Spatial transformer networks [[pdf]](https://arxiv.org/abs/1506.02025)
_Max Jaderberg, Karen Simonyan, Andrew Zisserman, and Koray Kavukcuoglu_
- The combination of the localisation network, grid generator, and sampler form a spatial transformer.

[[back to top]](#contents)

---

## Representation learning

### [ArXiv 2020] A Simple Framework for Contrastive Learning of Visual Representations [[pdf]](https://arxiv.org/abs/2002.05709)
_Ting Chen, Simon Kornblith, Mohammad Norouzi, Geoffrey Hinton_

### [ICLR 2020] Contrastive Representation Distillation [[pdf]](https://arxiv.org/abs/1910.10699)
_Yonglong Tian, Dilip Krishnan, Phillip Isola_
- Examples include distilling a large network into a smaller one, transferring knowledge from one sensory modality to a second, or ensembling a collection of models into a single estimator. **Knowledge distillation, the standard approach to these problems, minimizes the KL divergence between the probabilistic outputs of a teacher and student network.** We demonstrate that this objective ignores important structural knowledge of the teacher network. This motivates an alternative objective by which we train a student to capture significantly more information in the teacher’s representation of the data. We formulate this objective as contrastive learning. Experiments demonstrate that our resulting new objective outperforms knowledge distillation and other cutting-edge distillers on a variety of knowledge transfer tasks, including single model compression, ensemble distillation, and cross-modal transfer.
- Motivation: Representational knowledge is structured – the dimensions exhibit complex interdependencies. The original KD objective introduced in (Hinton et al., 2015, Distilling the knowledge in a neural network) treats all dimensions as independent, conditioned on the input.

### [ICLR 2020] Momentum Contrast for Unsupervised Visual Representation Learning [[pdf]](https://arxiv.org/abs/1911.05722)
_Kaiming He, Haoqi Fan, Yuxin Wu, Saining Xie, Ross Girshick_
- From a perspective on contrastive learning as dictionary look-up, we build a dynamic dictionary with a queue and a moving-averaged encoder. This enables building a large and consistent dictionary on-the-fly that facilitates contrastive unsupervised learning. This suggests that the gap between unsupervised and supervised representation learning has been largely closed in many vision tasks.
- The “keys” (tokens) in the dictionary are sampled from data (e.g., images or patches) and are represented by an encoder network. Unsupervised learning trains encoders to perform dictionary look-up: an encoded “query” should be similar to its matching key and dissimilar to others. Learning is formulated as minimizing a contrastive loss
- contrastive learning: Dimensionality reduction by learning an invariant mapping, CVPR 2006
- ![](../assets/fig_research_diary/1.PNG)

### [ICLR 2019] Learning deep representations by mutual information estimation and maximization [[pdf]](https://arxiv.org/abs/1808.06670)
_R Devon Hjelm, Alex Fedorov, Samuel Lavoie-Marchildon, Karan Grewal, Adam Trischler, and Yoshua Bengio_

### [ICCV 2019] Rethinking ImageNet pre-training [[pdf]](https://arxiv.org/abs/1811.08883)
_Kaiming He, Ross Girshick, Piotr Dollár_

### [NeurIPS] Learning Representations by Maximizing Mutual Information Across Views [[pdf]](https://arxiv.org/abs/1906.00910)
_Philip Bachman, R Devon Hjelm, William Buchwalter_

### [arXiv 2019] Data-Efficient Image Recognition with Contrastive Predictive Coding [[pdf]](https://arxiv.org/abs/1905.09272)
_Olivier J. Hénaff, Aravind Srinivas, Jeffrey De Fauw, Ali Razavi, Carl Doersch, S. M. Ali Eslami, Aaron van den Oord_

### [ICCV 2019] Local aggregation for unsupervised learning of visual embeddings [[pdf]](https://arxiv.org/abs/1903.12355)
_Chengxu Zhuang, Alex Lin Zhai, Daniel Yamins_

### [CVPR 2019] Self-Supervised Representation Learning by Rotation Feature Decoupling [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Feng_Self-Supervised_Representation_Learning_by_Rotation_Feature_Decoupling_CVPR_2019_paper.pdf)
_Zeyu Feng, Chang Xu, Dacheng Tao_
- ![](../assets/fig_research_diary/3.PNG)

### [CVPR 2018 spotlight] Unsupervised feature learning via non-parametric instance discrimination [[pdf]](https://arxiv.org/pdf/1805.01978v1.pdf)
_Zhirong Wu, Yuanjun Xiong, Stella Yu, and Dahua Lin_
- ![](../assets/fig_research_diary/2.PNG)
- noise constative estimation (NCE) and proximal regularization: \\(J_{NCE}(\theta) = -E_{P_d}\big[\log h(i, \mathbf{v}_i^{(t-1)}) - \lambda \|\mathbf{v}_i^{(t-1)}-\mathbf{v}_i^{(t)}\|_2^2 \big] - m\cdot E_{P_n}\big[\log (1-h(i, \mathbf{v'}^{(t-1)}))\big]\\). \\(P_d\\) means data distribution and \\(P_n\\) means noise distribution (uniform).

### [NeurIPS 2014] Discriminative unsupervised feature learning with convolutional neural networks [[pdf]](https://arxiv.org/abs/1406.6909)
_Alexey Dosovitskiy, Philipp Fischer, Jost Tobias Springenberg, Martin Riedmiller, Thomas Brox_

### [arXiv 2018] Representation learning with contrastive predictive coding [[pdf]](https://arxiv.org/abs/1807.03748)
_Aaron van den Oord, Yazhe Li, and Oriol Vinyals_

[[back to top]](#contents)

---

## Others

### [ICML 2020] Generalizing Convolutional Neural Networks for Equivariance to Lie Groups on Arbitrary Continuous Data [[pd]](https://arxiv.org/abs/2002.12880)
_Marc Finzi, Samuel Stanton, Pavel Izmailov, Andrew Gordon Wilson_

### [ICML 2020] Training Binary Neural Networks through Learning with Noisy Supervision [[pdf]](https://proceedings.icml.cc/static/paper_files/icml/2020/181-Paper.pdf)
_Kai Han, Yunhe Wang, Yixing Xu, Chunjing Xu, Enhua Wu, Chang Xu_

### [ICML 2020] Learning Flat Latent Manifolds with VAEs [[pd]](https://arxiv.org/abs/2002.04881)
_Nutan Chen, Alexej Klushyn, Francesco Ferroni, Justin Bayer, Patrick van der Smagt_

### [CVPR 2018] Neural 3D Mesh Renderer [[pdf]](https://arxiv.org/abs/1711.07566)
_Hiroharu Kato, Yoshitaka Ushiku, Tatsuya Harada_
- Therefore, in this work, we propose an approximate gradient for rasterization that enables the integration of rendering into neural networks.
- ![](../assets/fig_research_diary/11.PNG)

### [ICCV 2019] Deep Meta Metric Learning [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Deep_Meta_Metric_Learning_ICCV_2019_paper.pdf)
_Guangyi Chen, Tianren Zhang, Jiwen Lu, Jie Zhou_

### [AAAI 2020] Hybrid Graph Neural Networks for Crowd Counting [[pdf]](https://arxiv.org/abs/2002.00092)
_Ao Luo, Fan Yang, Xin Li, Dong Nie, Zhicheng Jiao, Shangchen Zhou, Hong Cheng_

### [ICLR 2020] Inductive Matrix Completion Based on Graph Neural Networks [[pdf]](https://arxiv.org/abs/1904.12058)
_Muhan Zhang, Yixin Chen_

### [NeurIPS] Quaternion Knowledge Graph Embeddings [[pdf]](https://arxiv.org/abs/1904.10281)
_Shuai Zhang, Yi Tay, Lina Yao, Qi Liu_

### [ICML 2019] EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks [[pdf]](https://arxiv.org/abs/1905.11946)
_Mingxing Tan, Quoc V. Le_

### [ICLR 2020] Geom-GCN: Geometric Graph Convolutional Networks [[pdf]](https://arxiv.org/abs/2002.05287)
_Hongbin Pei, Bingzhe Wei, Kevin Chen-Chuan Chang, Yu Lei, Bo Yang_
- Message-passing neural networks (MPNNs) have been successfully applied to representation learning on graphs in a variety of real-world applications. However, two fundamental weaknesses of MPNNs’ aggregators limit their ability to represent graph-structured data: **losing the structural information of nodes in neighborhoods and lacking the ability to capture long-range dependencies in disassortative graphs**. Few studies have noticed the weaknesses from different perspectives. From the observations on classical neural network and network geometry, we propose a novel geometric aggregation scheme for graph neural networks to overcome the two weaknesses. The behind basic idea is the aggregation on a graph can benefit from a continuous space underlying the graph. The proposed aggregation scheme is permutation-invariant and consists of three modules, node embedding, structural neighborhood, and bi-level aggregation.

### [NeurIPS 2019] General E(2) - Equivariant Steerable CNNs [[pdf]](https://arxiv.org/abs/1911.08251)
_Maurice Weiler, Gabriele Cesa_

### [CVPR 2020] DualConvMesh-Net: Joint Geodesic and Euclidean Convolutions on 3D Meshes [[pdf]](https://arxiv.org/abs/2004.01002)
_Jonas Schult, Francis Engelmann, Theodora Kontogianni, Bastian Leibe_

### [SIGGRAPH 2020] CNNs on Surfaces using Rotation-Equivariant Features [[pdf]](https://arxiv.org/abs/2006.01570)
_Ruben Wiersma, Elmar Eisemann, Klaus Hildebrandt_

### Accelerating 3D Deep Learning with PyTorch3D [[pdf]](https://arxiv.org/pdf/2007.08501)
_Nikhila Ravi, Jeremy Reizenstein, David Novotny, Taylor Gordon, Wan-Yen Lo, Justin Johnson, Georgia Gkioxari_

### On the Continuity of Rotation Representations in Neural Networks [[pdf]](https://arxiv.org/abs/1812.07035)
_Yi Zhou, Connelly Barnes, Jingwan Lu, Jimei Yang, Hao Li_

### [CVPR 2020] Adversarial Examples Improve Image Recognition [[pdf]](https://arxiv.org/abs/1911.09665)
_Cihang Xie, Mingxing Tan, Boqing Gong, Jiang Wang, Alan Yuille, Quoc V. Le_

### [NeurIPS 2020] A Closer Look at Accuracy vs. Robustness [[pdf]](https://arxiv.org/abs/2003.02460)
_Yao-Yuan Yang, Cyrus Rashtchian, Hongyang Zhang, Ruslan Salakhutdinov, Kamalika Chaudhuri_

### [ICML 2019] EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks [[pdf]](https://arxiv.org/abs/1905.11946)
_Mingxing Tan, Quoc V. Le_

[[back to top]](#contents)

---

## Transformer

### Spatially Sparse Convolution Library [[link]](https://github.com/traveller59/spconv)

### Submanifold Sparse Convolutional Networks [[link]](https://github.com/facebookresearch/SparseConvNet)

### [ICCV 2021] Voxel Transformer for 3D Object Detection [[pdf]](https://github.com/PointsCoder/VOTR)
_Jiageng Mao, Yujing Xue, Minzhe Niu, Haoyue Bai, Jiashi Feng, Xiaodan Liang, Hang Xu, Chunjing Xu_
- we propose the sparse voxel module and the submanifold voxel module, which can operate on the empty and non-empty voxel positions effectively.


### [ArXiv 2021] A Survey on Vision Transformer [[pdf]](https://arxiv.org/abs/2012.12556)
_Kai Han, Yunhe Wang, Hanting Chen, Xinghao Chen, Jianyuan Guo, Zhenhua Liu, Yehui Tang, An Xiao, Chunjing Xu, Yixing Xu, Zhaohui Yang, Yiman Zhang, Dacheng Tao_

### [ICCV 2021] Swin Transformer: Hierarchical Vision Transformer using Shifted Windows [[pdf]](https://arxiv.org/abs/2103.14030)
_Ze Liu, Yutong Lin, Yue Cao, Han Hu, Yixuan Wei, Zheng Zhang, Stephen Lin, Baining Guo_
 - ![](../assets/fig_transformer/12.png)
 - Relative position bias

### [CVPR 2021] Bottleneck Transformers for Visual Recognition [[pdf]](https://arxiv.org/abs/2101.11605)
_Aravind Srinivas, Tsung-Yi Lin, Niki Parmar, Jonathon Shlens, Pieter Abbeel, Ashish Vaswani_

### [ArXiv 2021] 3D Human Pose Estimation with Spatial and Temporal Transformers [[pdf]](https://arxiv.org/pdf/2103.10455.pdf)
_Ce Zheng, Sijie Zhu, Matias Mendieta, Taojiannan Yang, Chen Chen, Zhengming Ding_

### [NeurIPS 2021] Post-Training Quantization for Vision Transformer [[pdf]](https://arxiv.org/abs/2106.14156)
_Zhenhua Liu, Yunhe Wang, Kai Han, Siwei Ma, Wen Gao_

### [CVPR 2020] LiDAR-based Online 3D Video Object Detection with Graph-based Message Passing and Spatiotemporal Transformer Attention [[pdf]](https://arxiv.org/abs/2004.01389)
_Junbo Yin, Jianbing Shen, Chenye Guan, Dingfu Zhou, Ruigang Yang_

### [ArXiv 2021] Mesh Graphormer [[pdf]](https://arxiv.org/pdf/2104.00272.pdf)
_Kevin Lin, Lijuan Wang, Zicheng Liu_
 - ![](../assets/fig_transformer/8.png)

### [CVPR 2021] End-to-end human pose and mesh reconstruction with transformers [[pdf]](https://arxiv.org/pdf/2012.09760.pdf)
_Kevin Lin, Lijuan Wang, Zicheng Liu_
 - ![](../assets/fig_transformer/7.png)

### [ECCV 2020] Non-autoregressive structured modeling for 3d hand pose estimation [[pdf]](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123700018.pdf)
_Lin Huang, Jianchao Tan, Ji Liu, and Junsong Yuan_
 - ![](../assets/fig_transformer/6.png)

### [ArXiv 2021] CvT: Introducing Convolutions to Vision Transformers [[pdf]](https://arxiv.org/abs/2103.15808.pdf)
_Haiping Wu, Bin Xiao, Noel Codella, Mengchen Liu, Xiyang Dai, Lu Yuan, Lei Zhang_
 - ![](../assets/fig_transformer/9.png)
 - ![](../assets/fig_transformer/10.png)

### [ICCV 2021] Point transformer [[pdf]](https://arxiv.org/pdf/2012.09164.pdf)
_Hengshuang Zhao, Li Jiang, Jiaya Jia, Philip Torr, Vladlen Koltun_
 - ![](../assets/fig_transformer/11.png)

### [CVPR 2021] End-to-end video instance segmentation with transformers [[pdf]](https://arxiv.org/pdf/2011.14503.pdf)
_Yuqing Wang, Zhaoliang Xu, Xinlong Wang, Chunhua Shen, Baoshan Cheng, Hao Shen, Huaxia Xia_
 - ![](../assets/fig_transformer/5.png)

### [ArXiv 2021] A Survey on Visual Transformer [[pdf]](https://arxiv.org/abs/2012.12556.pdf)
_Kai Han, Yunhe Wang, Hanting Chen, Xinghao Chen, Jianyuan Guo, Zhenhua Liu, Yehui Tang, An Xiao, Chunjing Xu, Yixing Xu, Zhaohui Yang, Yiman Zhang, Dacheng Tao_

### [AAAI 2021] Informer: Beyond Efficient Transformer for Long Sequence Time-Series Forecasting [[pdf]](https://arxiv.org/abs/2012.07436.pdf)
_Haoyi Zhou, Shanghang Zhang, Jieqi Peng, Shuai Zhang, Jianxin Li, Hui Xiong, Wancai Zhang_

### [ECCV 2020] End-to-end object detection with transformers [[pdf]](https://arxiv.org/abs/2005.12872.pdf)
_Nicolas Carion, Francisco Massa, Gabriel Synnaeve, Nicolas Usunier, Alexander Kirillov, Sergey Zagoruyko_
 - ![](../assets/fig_transformer/4.png)

### [CVPR 2020] Actor-Transformers for Group Activity Recognition [[pdf]](https://arxiv.org/pdf/2003.12737.pdf)
_Kirill Gavrilyuk, Ryan Sanford, Mehrsan Javan, Cees G. M. Snoek_

### [ICLR 2021] An image is worth 16x16 words: Transformers for image recognition at scale [[pdf]](https://openreview.net/pdf?id=YicbFdNTTy)
_Alexey Dosovitskiy, Lucas Beyer, Alexander Kolesnikov, Dirk Weissenborn, Xiaohua Zhai, Thomas Unterthiner, Mostafa Dehghani, Matthias Minderer, Georg Heigold, Sylvain Gelly, Jakob Uszkoreit, Neil Houlsby_
 - ![](../assets/fig_transformer/3.png)

### [ICML 2020] Generative pretraining from pixels [[pdf]](https://cdn.openai.com/papers/Generative_Pretraining_from_Pixels_V2.pdf)
_Mark Chen, Alec Radford, Rewon Child, Jeffrey Wu, Heewoo Jun, David Luan, and Ilya Sutskever_
- ![](../assets/fig_transformer/2.png)

### [ArXiv 2020] Visual Transformers: Token-based Image Representation and Processing for Computer Vision [[pdf]](https://arxiv.org/pdf/2006.03677.pdf)
_Bichen Wu, Chenfeng Xu, Xiaoliang Dai, Alvin Wan, Peizhao Zhang, Zhicheng Yan, Masayoshi Tomizuka, Joseph Gonzalez, Kurt Keutzer, Peter Vajda_
- semantic segmentation with transformer
- ![](../assets/fig_transformer/1.png)

### [ICML 2018] Image transformer [[pdf]](https://arxiv.org/pdf/1802.05751.pdf)
_Niki Parmar, Ashish Vaswani, Jakob Uszkoreit, Łukasz Kaiser, Noam Shazeer, Alexander Ku, Dustin Tran_

[[back to top]](#contents)

---
