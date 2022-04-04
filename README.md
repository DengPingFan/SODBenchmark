# Salient objects in clutter (TPAMI2022-Minor)

> Authors:
> [Deng-Ping Fan](https://dengpingfan.github.io/), 
> [Jing Zhang](https://jingzhang617.github.io/), 
> [Gang Xu](https://github.com/CS-GangXu/), 
> [Ming-Ming Cheng](https://mmcheng.net/), 
> [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=zh-CN&oi=sra).

## 1. Preface

- This repository provides benchamrk for "_**Salient objects in clutter**_". 
([paper](https://arxiv.org/abs/2105.03053) | [中文版](https://dengpingfan.github.io/papers/[2022][TPAMI]SOC_Chinese.pdf))

- If you have any questions about our paper, feel free to contact me. And if you are using SOCbenchamrk results 
or evaluation toolbox for your research, please cite this paper ([BibTeX](#4-citation)).

## 2. Scope
Salient object detection (SOD) originated from the task of fixation prediction (FP), switching attention regions for accurate object-level regions. 
Current algorithms have been developed for 2D images of limited resolution (width or height $<$ 500 pixels), high-resolution (i.e., 1080p, 4K) and 
even remote sensing data. According to the supervision strategy, there are five types of SOD models: fully supervised, 
semi-supervised, weakly supervised, unsupervised, and self-supervised.

Recently, several interesting extensions of SOD have also been introduced, such as salient instance detection (SID), 
salient object subitizing (SOS), and saliency ranking. 
A taxonomy of the saliency detection task is shown below. 
Different from previous SOD reviews, we mainly focus on 2D salient object detection in a fully supervised manner. We highlight the scope of this study in gray.
For other closely related 3D/4D SOD tasks, we refer readers to
recent survey and benchmarking works such as RGB-D SOD, Event-RGB SOD [(ERSOD)](https://github.com/jxr326/ERSOD-Net), Light Field SOD,  
Co-SOD, 360° Video SOD, and Video SOD.
 
![avatar](Imgs/Scope.png)

## 2. 2D RGB Saliency Detection Models
## 2022       
**No.** | **Pub.** | **Title** | **Links** 
:-: | :-: | :-  | :-: 
01 | **AAAI** | Unsupervised Domain Adaptive Salient Object Detection Through Uncertainty-Aware Pseudo-Label Learning | [Paper](https://www.aaai.org/AAAI22Papers/AAAI-604.YanP.pdf)/[Code](https://github.com/Kinpzz/UDASOD-UPL)  
02 | **AAAI** | A Causal Debiasing Framework for Unsupervised Salient Object Detection | [Paper](https://www.aaai.org/AAAI22Papers/AAAI-108.LinX.pdf)/[Code]()  
03 | **AAAI** | Energy-Based Generative Cooperative Saliency Prediction | [Paper](https://www.aaai.org/AAAI22Papers/AAAI-1516.ZhangJ.pdf)/[Code](https://github.com/JingZhang617/SalCoopNets)  
04 | **AAAI** | Weakly-Supervised Salient Object Detection Using Point Supervison | [Paper](https://www.aaai.org/AAAI22Papers/AAAI-461.GaoS.pdf)/[Code](https://github.com/shuyonggao/PSOD)    
05 | **AAAI** | TRACER: Extreme Attention Guided Salient Object Tracing Network | [Paper](https://arxiv.org/pdf/2112.07380.pdf)/[Code](https://github.com/Karel911/TRACER)  
06 | **AAAI** | I can find you! Boundary-guided Separated Attention Network for Camouflaged Object Detection | [Paper](https://www.aaai.org/AAAI22Papers/AAAI-6565.ZhuH.pdf)/[Code](https://github.com/WolfberryCoke/BSA-Net)  
07 | **WACV** | Recursive Contour-Saliency Blending Network for Accurate Salient Object Detection | [Paper](https://openaccess.thecvf.com/content/WACV2022/papers/Ke_Recursive_Contour-Saliency_Blending_Network_for_Accurate_Salient_Object_Detection_WACV_2022_paper.pdf)/[Code](https://github.com/BarCodeReader/RCSB-PyTorch)  
08 | **IEEE TPAMI** | PoolNet+: Exploring the Potential of Pooling for Salient Object Detection | [Paper](https://mftp.mmcheng.net/Papers/21PAMI-PoolNet.pdf)/[Code](http://mmcheng.net/poolnet/)  
09 | **IEEE TPAMI** | A Highly Efficient Model to Study the Semantics of Salient Object Detection | [Paper](https://mftp.mmcheng.net/Papers/21PAMI-Sal100K.pdf)/[Code](https://mmcheng.net/sod100k/)  
10 | **IEEE TGRS** | Lightweight Salient Object Detection in Optical Remote Sensing Images via Feature Correlation | [Paper](https://arxiv.org/abs/2201.08049)/[Code](https://github.com/MathLee/CorrNet)  
11 | **TOMM** | Disentangle Saliency Detection into Cascaded Detail Modeling and Body Filling | [Paper](https://arxiv.org/pdf/2202.04112.pdf)/Code   
12 | **TMM** | Noise-Sensitive Adversarial Learning for Weakly Supervised Salient Object Detection | [Paper](https://ieeexplore.ieee.org/abstract/document/9716868/authors#authors)/[Code](https://github.com/wuweia123/IEEE-TMM-NSALWSS) 
13 | **ArXiv** | Joint Learning of Salient Object Detection, Depth Estimation and Contour Extraction | [Paper](https://arxiv.org/pdf/2203.04895.pdf)/Code 
14 | **ArXiv** | A Unified Transformer Framework for Group-based Segmentation: Co-Segmentation, Co-Saliency Detection and Video Salient Object Detection | [Paper](https://arxiv.org/pdf/2203.04708.pdf)/[Code](https://github.com/suyukun666/UFO) 
:triangular_flag_on_post: 18 | **IEEE TCyb** | Adjacent Context Coordination Network for Salient Object Detection in Optical Remote Sensing Images | [Paper](https://arxiv.org/pdf/2203.13664.pdf)/[Code](https://github.com/MathLee/ACCoNet) 


## 2021       
**No.** | **Pub.** | **Title** | **Links** 
:-: | :-: | :-  | :-: 
01 | **AAAI** | Structure-Consistent Weakly Supervised Salient Object Detection with Local Saliency Coherence | [Paper](https://arxiv.org/pdf/2012.04404.pdf)/[Code](https://github.com/siyueyu/SCWSSOD/tree/f8650567cbbc8df5bf6edc32a633c47a885574cd)
02 | **AAAI** | Pyramidal Feature Shrinking for Salient Object Detection | [Paper](https://www.aaai.org/AAAI21Papers/AAAI-1322.MaM.pdf)/[Code](https://github.com/iCVTEAM/PFSNet) 
03 | **AAAI** | Locate Globally, Segment Locally: A Progressive Architecture with Knowledge Review Network for Salient Object Detection | [Paper](https://www.aaai.org/AAAI21Papers/AAAI-4841.XuB.pdf)/[Code](https://github.com/bradleybin/Locate-Globally-Segment-locally-A-Progressive-Architecture-With-Knowledge-Review-Network-for-SOD)  
04 | **AAAI** | Multi-Scale Graph Fusion for Co-Saliency Detection | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/16951)/Code
05 | **AAAI** | Generating Diversified Comments via Reader-Aware Topic Modeling and Saliency Detection | [Paper](https://arxiv.org/pdf/2102.06856.pdf)/Code
06 | **ICIP** | Multiscale IoU: A Metric for Evaluation of Salient Object Detection with Fine Structures | [Paper](https://arxiv.org/pdf/2105.14572.pdf)/Code
07 | **TCSVT** | Weakly-Supervised Saliency Detection via Salient Object Subitizing | [Paper](https://arxiv.org/pdf/2101.00932.pdf)/Code 
08 | **TIP** | SAMNet: Stereoscopically Attentive Multi-scale Network for Lightweight Salient Object Detection | [Paper](https://ieeexplore.ieee.org/document/9381668)/[Code](https://github.com/yun-liu/FastSaliency) 
09 | **IJCAI** | C2FNet: Context-aware Cross-level Fusion Network for Camouflaged Object Detection | [Paper](https://arxiv.org/pdf/2105.12555.pdf)/[Code](https://github.com/thograce/C2FNet)
10 | **CVPR** | Railroad is not a Train: Saliency as Pseudo-pixel Supervision for Weakly Supervised Semantic Segmentation | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Lee_Railroad_Is_Not_a_Train_Saliency_As_Pseudo-Pixel_Supervision_for_CVPR_2021_paper.pdf)/[Code](https://github.com/halbielee/EPS)
11 | **CVPR** | Prototype-Guided Saliency Feature Learning for Person Search | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Kim_Prototype-Guided_Saliency_Feature_Learning_for_Person_Search_CVPR_2021_paper.pdf)/Code
12 | **CVPR** | Mesh Saliency: An Independent Perceptual Measure or A Derivative of Image Saliency? | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Song_Mesh_Saliency_An_Independent_Perceptual_Measure_or_a_Derivative_of_CVPR_2021_paper.pdf)/[Code](https://github.com/rsong/MIMO-GAN)
13 | **CVPR** | Weakly-Supervised Instance Segmentation via Class-Agnostic Learning With Salient Images | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_Weakly-Supervised_Instance_Segmentation_via_Class-Agnostic_Learning_With_Salient_Images_CVPR_2021_paper.pdf)/[Code](https://github.com/hustvl/BoxCaseg)
14 | **CVPR** | DeepACG: Co-Saliency Detection via Semantic-Aware Contrast Gromov-Wasserstein Distance | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_DeepACG_Co-Saliency_Detection_via_Semantic-Aware_Contrast_Gromov-Wasserstein_Distance_CVPR_2021_paper.pdf)/Code
15 | **CVPR** | Black-Box Explanation of Object Detectors via Saliency Maps | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Petsiuk_Black-Box_Explanation_of_Object_Detectors_via_Saliency_Maps_CVPR_2021_paper.pdf)/Code
16 | **CVPR** | From Semantic Categories to Fixations: A Novel Weakly-Supervised Visual-Auditory Saliency Detection Approach | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_From_Semantic_Categories_to_Fixations_A_Novel_Weakly-Supervised_Visual-Auditory_Saliency_CVPR_2021_paper.pdf)/[Code](https://github.com/guotaowang/STANet)
17 | **CVPR** | CAMERAS: Enhanced Resolution and Sanity Preserving Class Activation Mapping for Image Saliency | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Jalwana_CAMERAS_Enhanced_Resolution_and_Sanity_Preserving_Class_Activation_Mapping_for_CVPR_2021_paper.pdf)/[Code](https://github.com/VisMIL/CAMERAS)
18 | **CVPR** | Saliency-Guided Image Translation | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Jiang_Saliency-Guided_Image_Translation_CVPR_2021_paper.pdf)/Code
19 | **CVPR** | Group Collaborative Learning for Co-Salient Object Detection | [Paper](https://arxiv.org/pdf/2104.01108.pdf)/[Code](https://github.com/fanq15/GCoNet)
20 | **CVPR** | Uncertainty-aware Joint Salient Object and Camouflaged Object Detection | [Paper](https://arxiv.org/pdf/2104.02628.pdf)/[Code](https://github.com/JingZhang617/Joint_COD_SOD)
21 | **ACMM** | Auto-MSFNet: Search Multi-scale Fusion Network for Salient Object Detection | [Paper](https://github.com/LiuTingWed/Auto-MSFNet)/[Code](https://github.com/LiuTingWed/Auto-MSFNet) 
22 | **IEEE TIP** | Decomposition and Completion Network for Salient Object Detection | [Paper](https://ieeexplore.ieee.org/abstract/document/9479697/figures#figures)/[Code](https://github.com/wuzhe71/DCN) 
23 | **ICCV** | Visual Saliency Transformer | [Paper](https://arxiv.org/pdf/2104.12099.pdf)/[Code](https://github.com/nnizhang/VST#visual-saliency-transformer-vst) 
24 | **ICCV** | Disentangled High Quality Salient Object Detection | [Paper](https://arxiv.org/pdf/2108.03551.pdf)/[Code](https://github.com/luckybird1994/HQSOD) 
25 | **ICCV** | iNAS: Integral NAS for Device-Aware Salient Object Detection | [Paper](https://mftp.mmcheng.net/Papers/21ICCV-iNAS.pdf)/[Code](https://mmcheng.net/inas/) 
26 | **ICCV** | Scene Context-Aware Salient Object Detection | [Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Siris_Scene_Context-Aware_Salient_Object_Detection_ICCV_2021_paper.pdf)/[Code](https://github.com/SirisAvishek/Scene_Context_Aware_Saliency) 
27 | **ICCV** | MFNet: Multi-Filter Directive Network for Weakly Supervised Salient Object Detection | [Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Piao_MFNet_Multi-Filter_Directive_Network_for_Weakly_Supervised_Salient_Object_Detection_ICCV_2021_paper.pdf)/[Code](https://github.com/OIPLab-DUT/MFNet) 
28 | **ICCV** | Salient Object Ranking with Position-Preserved Attention | [Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Fang_Salient_Object_Ranking_With_Position-Preserved_Attention_ICCV_2021_paper.pdf)/[Code](https://github.com/EricFH/SOR) 
29 | **ICCV** | Summarize and Search: Learning Consensus-aware Dynamic Convolution for Co-Saliency Detection | [Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhang_Summarize_and_Search_Learning_Consensus-Aware_Dynamic_Convolution_for_Co-Saliency_Detection_ICCV_2021_paper.pdf)/[Code](https://github.com/nnizhang/CADC) 
30 | **IEEE TIP** | Salient Object Detection with Purificatory Mechanism and Structural Similarity Loss | [Paper](https://arxiv.org/pdf/1912.08393.pdf)/[Code](https://github.com/Jinming-Su/PurNet) 
31 | **ACMM** | Complementary Trilateral Decoder for Fast and Accurate Salient Object Detection | [Paper](https://dl.acm.org/doi/pdf/10.1145/3474085.3475494)/[Code](https://github.com/zhaozhirui/CTDNet)
32 | **NeurIPS** | Learning Generative Vision Transformer with Energy-Based Latent Space for Saliency Prediction | [Paper](https://proceedings.neurips.cc/paper/2021/file/8289889263db4a40463e3f358bb7c7a1-Paper.pdf)/Code   
33 | **NeurIPS** | Discovering Dynamic Salient Regions for Spatio-Temporal Graph Neural Networks | [Paper](https://proceedings.neurips.cc/paper/2021/file/398410ece9d7343091093a2a7f8ee381-Paper.pdf)/[Code](https://github.com/bit-ml/DyReg-GNN) 
34 | **IEEE TIP** | Progressive Self-Guided Loss for Salient Object Detection | [Paper](https://arxiv.org/pdf/2101.02412.pdf)/[Code](https://github.com/ysyscool/PSGLoss) 
35 | **IEEE TMM** | Dense Attention-guided Cascaded Network for Salient Object Detection of Strip Steel Surface Defects | [Paper](https://ieeexplore.ieee.org/document/9632537)/[Code](https://github.com/zxforchid/DACNet) 




## 2020       
**No.** | **Pub.** | **Title** | **Links** 
:-: | :-: | :-  | :-: 
01 | **AAAI** | Progressive Feature Polishing Network for Salient Object Detection | [Paper](https://arxiv.org/pdf/1911.05942.pdf)/[Code](https://github.com/chenquan-cq/PFPN)       
02 | **AAAI** | Global Context-Aware Progressive Aggregation Network for Salient Object Detection | [Paper](https://github.com/JosephChenHub/GCPANet/blob/master/GCPANet.pdf)/[Code](https://github.com/JosephChenHub/GCPANet)     
03 | **AAAI** | F3Net: Fusion, Feedback and Focus for Salient Object Detection | [Paper](https://arxiv.org/pdf/1911.11445.pdf)/[Code](https://github.com/weijun88/F3Net)    
04 | **AAAI** | Multi-spectral Salient Object Detection by Adversarial Domain Adaptation | [Paper](https://cse.sc.edu/~songwang/document/aaai20b.pdf)/Code 
05 | **AAAI** | Multi-Type Self-Attention Guided Degraded Saliency Detection | [Paper](https://cse.sc.edu/~songwang/document/aaai20a.pdf)/Code 
06 | **CVPR** | Weakly-Supervised Salient Object Detection via Scribble Annotations | [Paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_Weakly-Supervised_Salient_Object_Detection_via_Scribble_Annotations_CVPR_2020_paper.pdf)/[Code](https://github.com/JingZhang617/Scribble_Saliency)  
07 | **CVPR** | Taking a Deeper Look at the Co-salient Object Detection | [Paper](http://dpfan.net/wp-content/uploads/CoSalBenchmark_CVPR2020.pdf)/[Code](http://dpfan.net/CoSOD3K/)  
08 | **CVPR** | Multi-scale Interactive Network for Salient Object Detection | [Paper](https://drive.google.com/file/d/1gUYu0hO_8Xc5jgpzetuOVFDrqeSOiKZN/view?usp=sharing)/[Code](https://github.com/lartpang/MINet)  
09 | **CVPR** | Interactive Two-Stream Decoder for Accurate and Fast Saliency Detection | [Paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Zhou_Interactive_Two-Stream_Decoder_for_Accurate_and_Fast_Saliency_Detection_CVPR_2020_paper.pdf)/[Code](https://github.com/moothes/ITSD-pytorch)  
10 | **CVPR** | Label Decoupling Framework for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Wei_Label_Decoupling_Framework_for_Salient_Object_Detection_CVPR_2020_paper.pdf)/[Code](https://github.com/weijun88/LDF)  
11 | **CVPR** | Adaptive Graph Convolutional Network with Attention Graph Clustering for Co-saliency Detection | [Paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_Adaptive_Graph_Convolutional_Network_With_Attention_Graph_Clustering_for_Co-Saliency_CVPR_2020_paper.pdf)/Code
12 | **ECCV** | Highly Efficient Salient Object Detection with 100K Parameters | [Paper](http://mftp.mmcheng.net/Papers/20EccvSal100k.pdf)/[Code](https://github.com/MCG-NKU/Sal100K)
13 | **ECCV** | n-Reference Transfer Learning for Saliency Prediction | [Paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123530494.pdf)/[Code](https://github.com/luoyan407/n-reference)   
14 | **ECCV** | Gradient-Induced Co-Saliency Detection | [Paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123570443.pdf)/[Code](http://zhaozhang.net/coca.html)   
13 | **ECCV** | Learning Noise-Aware Encoder-Decoder from Noisy Labels by Alternating Back-Propagation for Saliency Detection | [Paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123620341.pdf)/[Code](https://github.com/JingZhang617/Noise-aware-ABP-Saliency)  
15 | **ECCV** | Suppress and Balance: A Simple Gated Network for Salient Object Detection | [Paper](https://arxiv.org/pdf/2007.08074.pdf)/[Code](https://github.com/Xiaoqi-Zhao-DLUT/GateNet-RGB-Saliency) 
16 | **IEEE TIP** | Dynamic Feature Integration for Simultaneous Detection of Salient Object, Edge and Skeleton | [Paper](http://mftp.mmcheng.net/Papers/20TIP-DFI.pdf)/[Code](https://github.com/backseason/DFI)
17 | **IEEE TIP** | CAGNet: Content-Aware Guidance for Salient Object Detection | [Paper](https://arxiv.org/abs/1911.13168)/[Code](https://github.com/Mehrdad-Noori/CAGNet)
18 | **IEEE TCYB** | Lightweight Salient Object Detection via Hierarchical Visual Perception Learning | [Paper](https://ieeexplore.ieee.org/document/9285193)/[Code](https://github.com/yun-liu/FastSaliency)
19 | **NeurIPS** | CoADNet: Collaborative Aggregation-and-Distribution Networks for Co-Salient Object Detection | [Paper](https://arxiv.org/pdf/2011.04887.pdf)/[Code](https://github.com/rmcong/CoADNet_NeurIPS20)
20 | **NeurIPS** | Few-Cost Salient Object Detection with Adversarial-Paced Learning | [Paper](https://papers.nips.cc/paper/2020/file/8fc687aa152e8199fe9e73304d407bca-Paper.pdf)/[Code](https://papers.nips.cc/paper/2020/file/8fc687aa152e8199fe9e73304d407bca-Supplemental.zip)
21 | **NeurIPS** | ICNet: Intra-saliency Correlation Network for Co-Saliency Detection | [Paper](https://proceedings.neurips.cc/paper/2020/file/d961e9f236177d65d21100592edb0769-Paper.pdf)/[Code](https://github.com/blanclist/ICNet)


  





## 2019       
**No.** | **Pub.** | **Title** | **Links** 
:-: | :-: | :-  | :-: 
01 | **CVPR** | AFNet: Attentive Feedback Network for Boundary-aware Salient Object Detection | [Paper](https://pan.baidu.com/s/1n-dRVC4sLWCmhhD5bnVXqg)/[Code](https://github.com/ArcherFMY/AFNet)  
02 | **CVPR** | BASNet: Boundary Aware Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_CVPR_2019/html/Qin_BASNet_Boundary-Aware_Salient_Object_Detection_CVPR_2019_paper.html)/[Code](https://github.com/NathanUA/BASNet) 
03 | **CVPR** | CPD: Cascaded Partial Decoder for Accurate and Fast Salient Object Detection | [Paper](https://arxiv.org/pdf/1904.08739.pdf)/[Code](https://github.com/wuzhe71/CPD-CVPR2019)
04 | **CVPR** | Multi-source weak supervision for saliency detection | [Paper](https://arxiv.org/pdf/1904.00566.pdf)/[Code](https://github.com/zengxianyu/mws)
05 | **CVPR** | MLMSNet:A Mutual Learning Method for Salient Object Detection with intertwined Multi-Supervision | [Paper](https://pan.baidu.com/s/1EUxabfnEi_l5-ghUI3_qVQ)/[Code](https://github.com/JosephineRabbit/MLMSNet)
06 | **CVPR** | CapSal: Leveraging Captioning to Boost Semantics for Salient Object Detection | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_CapSal_Leveraging_Captioning_to_Boost_Semantics_for_Salient_Object_Detection_CVPR_2019_paper.pdf)/[Code](https://github.com/zhangludl/code-and-dataset-for-CapSal)
07 | **CVPR** | PoolNet: A Simple Pooling-Based Design for Real-Time Salient Object Detection | [Paper](https://arxiv.org/pdf/1904.09569.pdf)/[Code](https://github.com/backseason/PoolNet) 
08 | **CVPR** | An Iterative and Cooperative Top-down and Bottom-up Inference Network for Salient Object Detection | [Paper](http://mftp.mmcheng.net/Papers/19cvprIterativeSOD.pdf)/Code
09 | **CVPR** | Pyramid Feature Attention Network for Saliency detection | [Paper](https://arxiv.org/pdf/1903.00179.pdf)/[Code](https://github.com/CaitinZhao/cvpr2019_Pyramid-Feature-Attention-Network-for-Saliency-detection)
10 | **AAAI** | Deep Embedding Features for Salient Object Detection | [Paper](https://pan.baidu.com/s/1HfyavmYB2NYUMe8CSe2qCw)/Code
11 | **ICIP** | Salient Object Detection Via Deep Hierarchical Context Aggregation And Multi-Layer Supervision | [Paper](https://github.com/ZhangC2/Saliency-DHCA-ML_S)/[Code](https://github.com/ZhangC2/Saliency-DHCA-ML_S)
12 | **IEEE TCSVT** | AADF-Net: Aggregating Attentional Dilated Features for Salient Object | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8836095)/[Code](https://github.com/githubBingoChen/AADF-Net)
13 | **IEEE TCyb** | ROSA: Robust Salient Object Detection against Adversarial Attacks | [Paper](https://arxiv.org/pdf/1905.03434.pdf)/[Code](https://github.com/lhaof/ROSA-Robust-Salient-Object-Detection-Against-Adversarial-Attacks)
14 | **arXiv** | DSAL-GAN: DENOISING BASED SALIENCY PREDICTION WITH GENERATIVE ADVERSARIAL NETWORKS | [Paper](https://arxiv.org/pdf/1904.01215.pdf)/Code
15 | **arXiv** | SAC-Net: Spatial Attenuation Context for Salient Object Detection | [Paper](https://arxiv.org/pdf/1903.10152.pdf)/Code
16 | **arXiv** | SE2Net: Siamese Edge-Enhancement Network for Salient Object Detection | [Paper](https://arxiv.org/pdf/1904.00048.pdf)/Code
17 | **arXiv** | Region Refinement Network for Salient Object Detection | [Paper](https://arxiv.org/pdf/1906.11443.pdf)/Code
18 | **arXiv** | Contour Loss: Boundary-Aware Learning for Salient Object Segmentation | [Paper](https://arxiv.org/pdf/1908.01975.pdf)/Code
19 | **arXiv** | OGNet: Salient Object Detection with Output-guided Attention Module | [Paper](https://arxiv.org/pdf/1907.07449.pdf)/Code
20 | **arXiv** | Edge-guided Non-local Fully Convolutional Network for Salient Object Detection | [Paper](https://arxiv.org/pdf/1908.02460.pdf)/Code
21 | **ICCV** | FLoss:Optimizing the F-measure for Threshold-free Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhao_Optimizing_the_F-Measure_for_Threshold-Free_Salient_Object_Detection_ICCV_2019_paper.pdf)/[Code](https://github.com/zeakey/iccv2019-fmeasure)
22  | **ICCV** | Stacked Cross Refinement Network for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Wu_Stacked_Cross_Refinement_Network_for_Edge-Aware_Salient_Object_Detection_ICCV_2019_paper.pdf)/[Code](https://github.com/wuzhe71/SCRN)
23 | **ICCV** | Selectivity or Invariance: Boundary-aware Salient Object Detection | [Paper](https://arxiv.org/pdf/1812.10066.pdf)/Code
24 | **ICCV** | HRSOD:Towards High-Resolution Salient Object Detection | [Paper](https://arxiv.org/pdf/1908.07274.pdf)/[Code](https://github.com/yi94code/HRSOD)
25 | **ICCV** | EGNet:Edge Guidance Network for Salient Object Detection | [Paper](http://mftp.mmcheng.net/Papers/19ICCV_EGNetSOD.pdf)/[Code](https://github.com/JXingZhao/EGNet)
26 | **ICCV** | Structured Modeling of Joint Deep Feature and Prediction Refinement for Salient Object Detection | [Paper](https://arxiv.org/pdf/1909.04366.pdf)/[Code](https://github.com/xuyingyue/DeepUnifiedCRF_iccv19)
27 | **ICCV** | Employing Deep Part-Object Relationships for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_Employing_Deep_Part-Object_Relationships_for_Salient_Object_Detection_ICCV_2019_paper.pdf)/Code
28 | **NeurIPS** | Deep Robust Unsupervised Saliency Prediction With Self-Supervision | [Paper](https://arxiv.org/pdf/1909.13055.pdf)/[Code](https://drive.google.com/file/d/10GlmenXR7nEJyRlmPHouvHP-g9KfUW1F/view)   
29 | **CVPR** | Salient Object Detection With Pyramid Attention and Salient Edges | [Paper](https://www.researchgate.net/publication/332751907_Salient_Object_Detection_With_Pyramid_Attention_and_Salient_Edges)/[Code](https://github.com/wenguanwang/PAGE-Net)      

    

## 2018
**No.** | **Pub.** | **Title** | **Links** 
:-: | :-: | :-  | :-: 
01 | **CVPR** | A Bi-Directional Message Passing Model for Salient Object Detection | [Paper](https://pan.baidu.com/s/1akKVVipD8vIIv0XFrWND5Q)/[Code](https://github.com/zhangludl/A-bi-directional-message-passing-model-for-salient-object-detection)  
02 | **CVPR** | PiCANet: Learning Pixel-wise Contextual Attention for Saliency Detection | [Paper](http://arxiv.org/abs/1708.06433)/[Code](https://github.com/Ugness/PiCANet-Implementation)
03 | **CVPR** | PAGR: Progressive Attention Guided Recurrent Network for Salient Object Detection | [Paper](https://github.com/zhangxiaoning666/PAGR)/[Code](https://github.com/yangbinb/SalMetric/tree/master/PAGRN)
04 | **CVPR** | Learning to promote saliency detectors | [Paper](https://pan.baidu.com/s/1QvDmqruH8oU51_GrgsuXoA)/[Code](https://github.com/zengxianyu/lps)
05 | **CVPR** | Detect Globally, Refine Locally: A Novel Approach to Saliency Detection | [Paper](https://pan.baidu.com/s/1ydLI0koPfndehqMOAwrK_Q)/[Code](https://github.com/TiantianWang/CVPR18_detect_globally_refine_locally)
06 | **CVPR** | Salient Object Detection Driven by Fixation Prediction | [Paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wang_Salient_Object_Detection_CVPR_2018_paper.pdf)/[Code](https://github.com/wenguanwang/ASNet)
07 | **IJCAI** | R3Net: Recurrent Residual Refinement Network for Saliency Detection | [Paper](https://www.ijcai.org/proceedings/2018/0095.pdf)/[Code](https://github.com/zijundeng/R3Net)
08 | **IJCAI** | LFR: Salient Object Detection by Lossless Feature Reflection | [Paper](https://pan.baidu.com/s/1DAyPHe_z0LJpKK8DxKF2dg)/[Code](https://github.com/Pchank/caffe-sal/blob/master/IIAU2018.md)
09 | **ECCV** | Contour Knowledge Transfer for Salient Object Detection | [Paper](http://link-springer-com-s.vpn.whu.edu.cn:9440/content/pdf/10.1007/978-3-030-01267-0_22.pdf)/[Code](https://github.com/lixin666/C2SNet)
10 | **ECCV** | Reverse Attention for Salient Object Detection | [Paper](http://arxiv.org/pdf/1807.09940)/[Code](https://github.com/ShuhanChen/RAS_ECCV18)
11 | **IEEE TIP** | An unsupervised game-theoretic approach to saliency detection | [Paper](https://pan.baidu.com/s/1U1O4oFK6ZALSghPjJv_5nA)/[Code](https://github.com/zengxianyu/uga)
12 | **arXiv** | Agile Amulet: Real-Time Salient Object Detection with Contextual Attention | [Paper](http://arxiv.org/pdf/1802.06960)/[Code](https://github.com/Pchank/caffe-sal/blob/master/IIAU2018.md)
13 | **arXiv** | HyperFusion-Net: Densely Reflective Fusion for Salient Object Detection | [Paper](http://arxiv.org/pdf/1804.05142)/[Code](https://github.com/Pchank/caffe-sal/blob/master/IIAU2018.md)
14 | **arXiv** | (TBOS)Three Birds One Stone: A Unified Framework for Salient Object Segmentation, Edge Detection and Skeleton Extraction | [Paper](https://arxiv.org/pdf/1803.09860.pdf)/Code
15 | **CVPR** | Deep Unsupervised Saliency Detection: A Multiple Noisy Labeling Perspective | [Paper](https://arxiv.org/abs/1803.10910)/[Code](https://github.com/kris-singh/Deep-Unsupervised-Saliency-Detection)


    
 
## 2017
**No.** | **Pub.** | **Title** | **Links** 
:-: | :-: | :-  | :-: 
01 | **CVPR** | DSS: Deeply Supervised Salient Object Detection with Short Connections | [Paper](http://arxiv.org/abs/1611.04849)/[Code](https://github.com/Andrew-Qibin/DSS)
02 | **CVPR** | Non-Local Deep Features for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Luo_Non-Local_Deep_Features_CVPR_2017_paper.pdf)/[Code](https://github.com/zhimingluo/NLDF)
03 | **CVPR** | Learning to Detect Salient Objects with Image-level Supervision | [Paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Wang_Learning_to_Detect_CVPR_2017_paper.pdf)/[Code](https://github.com/scott89/WSS)
04 | **CVPR** | SalGAN: visual saliency prediction with adversarial networks | [Paper](http://arxiv.org/abs/1701.01081)/[Code](https://github.com/Pchank/caffe-sal)
05 | **ICCV** | A Stagewise Refinement Model for Detecting Salient Objects in Images | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Wang_A_Stagewise_Refinement_ICCV_2017_paper.pdf)/[Code](https://github.com/Pchank/caffe-sal)
06 | **ICCV** | Amulet: Aggregating Multi-level Convolutional Features for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhang_Amulet_Aggregating_Multi-Level_ICCV_2017_paper.pdf)/[Code](https://github.com/Pchank/caffe-sal)
07 | **ICCV** | Learning Uncertain Convolutional Features for Accurate Saliency Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhang_Learning_Uncertain_Convolutional_ICCV_2017_paper.pdf)/[Code](https://github.com/Pchank/caffe-sal)
08 | **ICCV** | Supervision by Fusion: Towards Unsupervised Learning of Deep Salient Object Detector  | [Paper](https://openaccess.thecvf.com/content_ICCV_2017/papers/Zhang_Supervision_by_Fusion_ICCV_2017_paper.pdf)/[Code](https://github.com/zhangyuygss/SVFSal.caffe)

 
  

## 2016
**No.** | **Pub.** | **Title** | **Links** 
:-: | :-: | :-  | :-: 
01 | **CVPR** | DHSNet: Deep hierarchical saliency network for salient object detection | [Paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Liu_DHSNet_Deep_Hierarchical_CVPR_2016_paper.pdf)/[Code](https://github.com/GuanWenlong/DHSNet-PyTorch)
02 | **CVPR** | ELD: Deep Saliency with Encoded Low level Distance Map and High Level Features | [Paper](http://www.arxiv.org/pdf/1604.05495v1.pdf)/[Code](https://github.com/gylee1103/SaliencyELD)
03 | **ECCV** | RFCN: Saliency detection with recurrent fully convolutional networks | [Paper](http://202.118.75.4/lu/Paper/ECCV2016/0865.pdf)/[Code](https://github.com/zengxianyu/RFCN)

