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

## Traditional Methods (Updated: 2022-04-04)
 **No.** | **Name.** |    **Pub.**    | **Year** | **Title**                                                    |                          **Links**                           
:-: | :-: | :-: | :-: | :-  | :-: 
   01    |    It     |     TPAMI      |   1998   | A Model of Saliency-Based Visual Attention for Rapid Scene Analysis | [[Paper](https://www.researchgate.net/publication/3192913_A_Model_of_Saliency-based_Visual_Attention_for_Rapid_Scene_Analysis)]/[Code] 
   02    |    FG     |     ACMMM      |   2003   | Contrast-based image attention analysis by using fuzzy growing | [[Paper](https://dl.acm.org/doi/abs/10.1145/957013.957094)]/[Code] 
   03    |    RSA    |     ACMMM      |   2005   | Robust subspace analysis for detecting visual attention regions in images | [[Paper](https://dl.acm.org/doi/10.1145/1101149.1101306)]/[Code] 
   04    |    AIM    |    NeurIPS     |   2005   | Saliency Based on Information Maximization                   | [[Paper](https://proceedings.neurips.cc/paper/2005/file/0738069b244a1c43c83112b735140a16-Paper.pdf)]/[Code] 
   05    |    RE     |      ICME      |   2006   | Region enhanced scale-invariant saliency detection           | [[Paper](https://graphics.cs.wisc.edu/Papers/2006/LG06a/imgsal.pdf)]/[Code] 
   06    |    SR     |      CVPR      |   2007   | Saliency Detection A Spectral Residual Approach              | [[Paper](https://www.researchgate.net/publication/221364530_Saliency_Detection_A_Spectral_Residual_Approach)]/[[Code](https://github.com/uoip/SpectralResidualSaliency)] 
   07    |    GB     |    NeurIPS     |   2007   | Graph-Based Visual Saliency                                  | [[Paper](https://proceedings.neurips.cc/paper/2006/file/4db0f8b0fc895da263fd77fc8aecabe4-Paper.pdf)]/[[Code](https://github.com/shreelock/gbvs)] 
   08    |    RU     |      TMM       |   2007   | A rule based technique for extraction of visual attention regions based on real-time clustering | [[Paper](https://www.researchgate.net/publication/3424588_A_Rule_Based_Technique_for_Extraction_of_Visual_Attention_Regions_Based_on_Real-Time_Clustering)]/[Code] 
   09    |    SUN    |      JOV       |   2008   | SUN: A bayesian framework for saliency using natural statistics | [[Paper](https://cseweb.ucsd.edu/~gary/pubs/Zhang-et-al-2008-accepted.pdf)]/[[Code](https://github.com/wohlert/bayesian-saliency)] 
   10    |    AC     |      ICVS      |   2008   | Salient region detection and segmentation                    | [[Paper](http://www.cs.toronto.edu/~strider/publications/AES_ICVS08.pdf)]/[[Code](https://github.com/assamite/sdrs_cimg)] 
   11    |    FT     |      CVPR      |   2009   | Frequency-tuned Salient Region Detection                     | [[Paper](http://projectsweb.cs.washington.edu/research/insects/CVPR2009/features/freqtuned_salient_regdetect.pdf)]/[[Code](https://github.com/liaoxl/Frequency-Tuned-Saliency-and-Segment)] 
   12    |    ICC    |      ICCV      |   2009   | Image saliency by isocentric curvedness and color            | [[Paper](https://www.researchgate.net/publication/224135956_Image_saliency_by_isocentric_curvedness_and_color)]/[Code] 
   13    |    EDS    |       PR       |   2009   | A simple method for detecting salient regions                | [[Paper](https://www.researchgate.net/publication/223277930_A_simple_method_for_detecting_salient_regions)]/[Code] 
   14    |    CA     |      CVPR      |   2010   | Context-Aware Saliency Detection                             | [[Paper](https://www.researchgate.net/publication/51925347_Context-Aware_Saliency_Detection)]/[[Code](https://github.com/Somefive/context-aware-saliency-detection)] 
   15    |    SEG    |      ECCV      |   2010   | Segmenting Salient Objects from Images and Videos            | [[Paper](http://users.jyu.fi/~salomi/pub/ECCV2010_Cameraready.pdf)]/[Code] 
   16    |   MSSS    |      ICIP      |   2010   | Saliency Detection using Maximum Symmetric Surround          | [[Paper](https://infoscience.epfl.ch/record/151989)]/[[Code](https://www.epfl.ch/labs/ivrl/research/saliency/saliency-msss/)] 
   17    |    CSM    |     ACMMM      |   2010   | Automatic interesting object extraction from images using complementary saliency maps | [[Paper](https://www.researchgate.net/publication/221573194_Automatic_interesting_object_extraction_from_images_using_complementary_saliency_maps)]/[Code] 
   18    |   HC,RC   |      CVPR      |   2011   | Global Contrast based Salient Region Detection               | [[Paper](https://mmcheng.net/mftp/Papers/SaliencyTPAMI.pdf)]/[[Code](https://github.com/congve1/SaliencyRC)] 
   19    |    SVO    |      ICCV      |   2011   | Fusing generic objectness and visual saliency for salient object detection | [[Paper](https://homepage.iis.sinica.edu.tw/papers/liutyng/12853-F.pdf)]/[[Code](https://homepage.iis.sinica.edu.tw/~liutyng/Projects/ObjSal/)] 
   20    |    CSD    |      ICCV      |   2011   | Center-surround divergence of feature statistics for salient object detection | [[Paper](https://www.researchgate.net/publication/221110022_Center-surround_divergence_of_feature_statistics_for_salient_object_detection)]/[Code] 
   21    |    CC     |      ICCV      |   2011   | Salient object detection using concavity context             | [[Paper](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.716.854&rep=rep1&type=pdf)]/[Code] 
   22    |    CB     |      BMVC      |   2011   | Automatic Salient Object Segmentation Based on Context and Shape Prior | [[Paper](https://jingdongwang2017.github.io/Pubs/BMVC11-Salient.pdf)]/[[Code](https://github.com/zhfe99/sal/tree/master/tool/2011_BMVC_CBSaliency)] 
   23    |    SF     |      CVPR      |   2012   | Saliency Filters Contrast Based Filtering for Salient Region Detection | [[Paper](https://fperazzi.github.io/projects/saliency_filters/)]/[[Code](https://fperazzi.github.io/projects/saliency_filters/)] 
   24    |    LR     |      CVPR      |   2012   | A Unified Approach to Salient Object Detection via Low Rank Matrix Recovery | [[Paper](https://xiaohuishen.github.io/assets/saliency_cvpr12.pdf)]/[Code] 
   25    |    GS     |      ECCV      |   2012   | Geodesic saliency using background priors                    | [[Paper](http://jiansun.org/papers/ECCV12_GeodesicSaliency.pdf)]/[[Code](https://github.com/garyzhao/SaliencyBaseline)] 
   26    |    BSF    |      ICIP      |   2012   | Saliency Detection Based on Integration of Boundary and Soft-Segmentation | [[Paper](https://ieeexplore.ieee.org/abstract/document/6467052)]/[[Code](https://github.com/huchuanlu/12_13)] 
   27    |   GC,GU   |      ICCV      |   2013   | Efficient Salient Region Detection with Soft Image Abstraction | [[Paper](https://www.researchgate.net/publication/257959398_Efficient_Salient_Region_Detection_with_Soft_Image_Abstraction)]/[[Code](https://github.com/MCG-NKU/CmCode)] 
   28    |    MR     |      CVPR      |   2013   | Saliency Detection via Graph-Based Manifold Ranking          | [[Paper](https://openaccess.thecvf.com/content_cvpr_2013/papers/Yang_Saliency_Detection_via_2013_CVPR_paper.pdf)]/[[Code](https://github.com/ruanxiang/mr_saliency)] 
   29    |    MC     |      ICCV      |   2013   | Saliency Detection via Absorbing Markov Chain                | [[Paper](https://faculty.ucmerced.edu/mhyang/papers/iccv13_saliency2.pdf)]/[[Code](https://github.com/lihezhang-dut/AMC_AE)] 
   30    |   DRFI    |      CVPR      |   2013   | Salient Object Detection A Discriminative Regional Feature Integration Approach | [[Paper](https://arxiv.org/pdf/1410.5926.pdf)]/[[Code](https://github.com/playerkk/drfi_matlab)] 
   31    |    DSR    |      ICCV      |   2013   | Saliency Detection via Dense and Sparse Reconstruction       | [[Paper](https://faculty.ucmerced.edu/mhyang/papers/iccv13_saliency1.pdf)]/[[Code](https://github.com/huchuanlu/13_1)] 
   32    |   PISA    |      CVPR      |   2013   | Pisa: Pixelwise image saliency by aggregating complementary appearance contrast measures with spatial priors | [[Paper](https://www.researchgate.net/publication/261263630_PISA_Pixelwise_Image_Saliency_by_Aggregating_Complementary_Appearance_Contrast_Measures_With_Spatial_Priors)]/[Code] 
   33    |    CRF    |      CVPR      |   2013   | Saliency aggregation: A data-driven approach                 | [[Paper](https://openaccess.thecvf.com/content_cvpr_2013/papers/Mai_Saliency_Aggregation_A_2013_CVPR_paper.pdf)]/[[Code](http://web.cecs.pdx.edu/~fliu/project/saliency-aggregation/)] 
   34    |    HS     |      CVPR      |   2013   | Hierarchical Saliency Detection                              | [[Paper](https://openaccess.thecvf.com/content_cvpr_2013/papers/Yan_Hierarchical_Saliency_Detection_2013_CVPR_paper.pdf)]/[Code] 
   35    |    PCA    |      CVPR      |   2013   | What Makes a Patch Distinct                                  | [[Paper](https://openaccess.thecvf.com/content_cvpr_2013/papers/Margolin_What_Makes_a_2013_CVPR_paper.pdf)]/[Code] 
   36    |    STD    |      CVPR      |   2013   | Statistical textural distinctiveness for salient region detection in natural images | [[Paper](https://openaccess.thecvf.com/content_cvpr_2013/papers/Scharfenberger_Statistical_Textural_Distinctiveness_2013_CVPR_paper.pdf)]/[Code] 
   38    |    SUB    |      CVPR      |   2013   | Submodular salient region detection                          | [[Paper](https://openaccess.thecvf.com/content_cvpr_2013/papers/Jiang_Submodular_Salient_Region_2013_CVPR_paper.pdf)]/[Code] 
   39    |    UFO    |      ICCV      |   2013   | Salient Region Detection by UFO Uniqueness, Focusness and Objectness | [[Paper](https://www.yumpu.com/en/document/read/51454544/salient-region-detection-by-ufo-uniqueness-temple-university)]/[Code] 
   40    |    CHM    |      ICCV      |   2013   | Contextual hypergraph modeling for salient object detection  | [[Paper](https://openaccess.thecvf.com/content_iccv_2013/papers/Li_Contextual_Hypergraph_Modeling_2013_ICCV_paper.pdf)]/[[Code](https://cs.adelaide.edu.au/~yaoli/?page_id=149)] 
   41    |    COV    |      JOV       |   2013   | Visual saliency estimation by nonlinearly integrating features using region covariances | [[Paper](https://jov.arvojournals.org/article.aspx?articleid=2121371)]/[Code] 
   42    |    CIO    |      ICCV      |   2013   | Category-independent object-level saliency detection         | [[Paper](https://www.yumpu.com/en/document/read/22480605/category-independent-object-level-saliency-detection)]/[Code] 
   43    |    GR     |      SPL       |   2013   | Graph-Regularized Saliency Detection With Convex-Hull-Based Center Prior | [[Paper](https://www.researchgate.net/publication/260328532_Graph-Regularized_Saliency_Detection_With_Convex-Hull-Based_Center_Prior)]/[[Code](https://github.com/MCG-NKU/SalBenchmark/tree/master/Code/matlab/GR)] 
   44    |   SLMR    |      BMVC      |   2013   | Segmentation driven lowrank matrix recovery for saliency detection | [[Paper](http://www.bmva.org/bmvc/2013/Papers/paper0078/abstract0078.pdf)]/[Code] 
   45    |   LSSC    |      TIP       |   2013   | Bayesian Saliency via Low and Mid Level Cues                 | [[Paper](https://pan.baidu.com/s/1BUVZmFj_P7o44f35_7lx-w?_at_=1649102618858)]/[[Code](https://github.com/huchuanlu/13_6)] 
   46    |   LSMD    |      AAAI      |   2013   | Salient object detection via low-rank and structured sparse matrix decomposition | [[Paper](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.978.9744&rep=rep1&type=pdf)]/[Code] 
   47    |   HDCT    |      CVPR      |   2014   | Salient Region Detection via High-Dimensional Color Transform | [[Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Kim_Salient_Region_Detection_2014_CVPR_paper.pdf)]/[[Code](https://github.com/jhkim89/Saliency-HDCT)] 
   48    |    PDE    |      CVPR      |   2014   | Adaptive partial differential equation learning for visual saliency detection | [[Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Liu_Adaptive_Partial_Differential_2014_CVPR_paper.pdf)]/[Code] 
   49    |    RBD    |      CVPR      |   2014   | Saliency Optimization from Robust Background Detection       | [[Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Zhu_Saliency_Optimization_from_2014_CVPR_paper.pdf)]/[[Code](https://github.com/yhenon/pyimgsaliency)] 
   50    |    MSS    |      SPL       |   2014   | Saliency Detection with Multi-Scale Superpixels              | [[Paper](https://www.researchgate.net/publication/262417209_Saliency_Detection_with_Multi-Scale_Superpixels)]/[Code] 
   51    |    GP     |      ICCV      |   2015   | Generic Promotion of Diffusion-Based Salient Object Detection | [[Paper](https://openaccess.thecvf.com/content_iccv_2015/papers/Jiang_Generic_Promotion_of_ICCV_2015_paper.pdf)]/[Code] 
   52    |    MBS    |      ICCV      |   2015   | Minimum Barrier Salient Object Detection at 80 FPS           | [[Paper](https://cs-people.bu.edu/jmzhang/fastmbd/MBS_preprint.pdf)]/[[Code](https://github.com/jimmie33/MBS)] 
   53    |    WSC    |      CVPR      |   2015   | A Weighted Sparse Coding Framework for Saliency Detection    | [[Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Li_A_Weighted_Sparse_2015_CVPR_paper.pdf)]/[[Code](https://www.eecis.udel.edu/~nianyi/WSC.html)] 
   54    |    RRW    |      CVPR      |   2015   | Robust saliency detection via regularized random walks ranking | [[Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2015/ext/2A_053_ext.pdf)]/[[Code](https://github.com/yuanyc06/rr)] 
   55    |   TLLT    |      CVPR      |   2015   | Saliency Propagation from Simple to Difficult                | [[Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Gong_Saliency_Propagation_From_2015_CVPR_paper.pdf)]/[Code] 
   56    |    BL     |      CVPR      |   2015   | Salient Object Detection via Bootstrap Learning              | [[Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Tong_Salient_Object_Detection_2015_CVPR_paper.pdf)]/[[Code](https://github.com/huchuanlu/15_4)] 
   57    |   BSCA    |      CVPR      |   2015   | Saliency Detection via Cellular Automata                     | [[Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Qin_Saliency_Detection_via_2015_CVPR_paper.pdf)]/[[Code](https://github.com/huchuanlu/15_2)] 
   58    |    GLC    |       PR       |   2015   | Salient Object Detection via Global and Local Cues           | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320314004932)]/[[Code](https://sciencenest.com/downloads/salient-object-detection-via-global-and-local-cues/)] 
   59    |    LPS    |      TIP       |   2015   | Inner and Inter Label Propagation Salient Object Detection in the Wild | [[Paper](https://arxiv.org/abs/1505.07192)]/[[Code](https://github.com/hli2020/lps_tip15)] 
   60    |   MAPM    |      TIP       |   2015   | Saliency Region Detection based on Markov Absorption Probabilities | [[Paper](https://ieeexplore.ieee.org/document/7041218)]/[Code] 
   61    |    NCS    |      TIP       |   2015   | Normalized cut-based saliency detection by adaptive multi-level region merging | [[Paper](https://gcatnjust.github.io/ChenGong/paper/fu_tip15.pdf)]/[[Code](https://www.kerenfu.top/sources/TIPdemo.zip)] 
   62    |    BFS    |       NC       |   2015   | Saliency Detection via Background and Foreground Seed Selection | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0925231214014416?via%3Dihub)]/[Code] 
   63    |    UF     |      TMM       |   2016   | A Universal Framework for Salient Object Detection           | [[Paper](http://sim.jxufe.cn/JDMKL/pdf/A%20universal%20framework%20for%20salient%20object%20detection.pdf)]/[Code] 
   64    |    MST    |      CVPR      |   2016   | Real-Time Salient Object Detection with a Minimum Spanning Tree | [[Paper](https://openaccess.thecvf.com/content_cvpr_2016/papers/Tu_Real-Time_Salient_Object_CVPR_2016_paper.pdf)]/[[Code](https://github.com/lhaof/Real-Time-Salient-Object-Detection-with-a-Minimum-Spanning-Tree)] 
   65    |    PM     |      ECCV      |   2016   | Pattern Mining Saliency                                      | [[Paper](https://link.springer.com/chapter/10.1007/978-3-319-46466-4_35)]/[[Code](https://github.com/huchuanlu/16_3)] 
   66    |    DSP    |       PR       |   2016   | Discriminative saliency propagation with sink points         | [[Paper](http://shuhanchen.net/papers/PR16.pdf)]/[[Code](https://github.com/ShuhanChen/DSP_PR2016)] 
   67    |    EBM    |     IJCAI      |   2016   | Saliency Transfer: An Example-Based Method for Salient Object Detection | [[Paper](https://www.ijcai.org/Proceedings/16/Papers/482.pdf)]/[Code] 
   68    |    AWC    | Neurocomputing |   2016   | Robust manifold-preserving diffusion-based saliency detection by adaptive weight construction | [[Paper](http://www.kerenfu.top/sources/NEUCOM_2016.pdf)]/[[Code](https://www.kerenfu.top/sources/MPDS.zip)] 
   69    |   MRMF    |     TNNLS      |   2016   | Manifold Ranking-Based Matrix Factorization for Saliency Detection | [[Paper](https://ieeexplore.ieee.org/iel7/5962385/6104215/07185439.pdf)]/[Code] 
   70    |   SBCRF   | Neurocomputing |   2017   | A superpixel-based CRF saliency detection approach           | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0925231217305118)]/[Code] 
   71    |   WLRR    |      SPL       |   2017   | Salient Object Detection via Weighted Low Rank Matrix Recovery | [[Paper](https://ieeexplore.ieee.org/document/7605498)]/[Code] 
   72    |    MIL    |      TIP       |   2017   | Salient Object Detection via Multiple Instance Learning      | [[Paper](http://faculty.dlut.edu.cn/system/resource/tsites/download.jsp?ap=lwyfj&fl=Zr2IVvVZVjEr&uid=5469&fid=BYMV6RNXYMXPAMWV74AALKADTHZBSVM4)]/[Code] 
   73    |    SMD    |      PAMI      |   2017   | Salient Object Detection via Structured Matrix Decomposition | [[Paper](https://ieeexplore.ieee.org/document/7464858)]/[Code] 
   74    |    MDC    |      TIP       |   2017   | 300-FPS Salient Object Detection via Minimum Directional Contrast | [[Paper](http://ieeexplore.ieee.org/document/7937833/)]/[[Code](https://github.com/huangxm14-thu/SaliencyMDC)] 
   75    |    SS     |       NC       |   2017   | Spectral Salient Object Detection                            | [[Paper](https://pdf.sciencedirectassets.com/271597/1-s2.0-S0925231217X00489/1-s2.0-S0925231217315412/am.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEPH%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJIMEYCIQDiB%2FAORBeokjPDtN%2F67MgjGm9CUMihfg82HmpjkwB3KwIhAJ8uaSK9fbc94N71ER4anEpu6qHNBWwLdIVfmhdk1iliKoMECIr%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEQBBoMMDU5MDAzNTQ2ODY1IgzlawP9%2BbyGIJMNKSsq1wMsp%2FLDWiHF3a%2B5BZEctcxm0fB68tO0bT8HPY2KxK0ytFV0METt%2ByKVdjSrXahUM1226ueCP2gicV%2BpfqKV3XCv0XCYf5tvYX47A3Pdek%2BipyREpFkeMOrdej5Lk%2FrNDFt52YWOUHtiTv1BlbXzojwWmIsiwjotWhsH8%2Fm1SGGaIKDQALqBu5BPBRLraivAirK8rNhAzT%2Bf%2FD0T%2F9SnW6lq79Qw9g%2Bm%2FeFrO86N3T31g0xae9RtJG6gBTMVwdjXSSLi0HW2ReX26frReIh%2Fb2KncBS7ie1ZTkQM4P0jSyhTj2AzvP%2Bln5T19W%2FtonXsU3LkyBKrmfJuwkFVAUdpqv36SwAnIqdMcIP%2FZJG6%2BpHE3EbRMrm1A5yIUQu15wBKzVG%2F6lYhncPalamwQPxZ3tmtQvqKPg97UlDI6ne%2FCzBXDxprEr6mAHxZjyRkPOS5wp4tMTylMgbSM5REGaAGRn3mPF8IikzO9tFdkUwI%2B8Zs9JN3dBZj8LJUAfdSG8nyye3AIxu3AnmAmD0APst95eKHOH%2FKC8nf6DqyCtSdtdQLBI4eZkOKQPwni0fiI0gm9HSf4vvfAl9acpU8lzBae%2FzdF6%2Fr7pTtFYcMOrZaQUSekjEBrcVsiLYwloiwkgY6pAEsxQS6Ct%2FtsL1EQeKqmhSTyZvejoLoZovjng2XS%2BAFsxZvXk5jVZu6Hb0c9T94p0egnHjV2TvTA6wE2i7mb0sP0EI4WKHv7l1dwI73wzgo%2Fe4t32DxcoatqjiqnwzEXrMNUMG7MU2%2FLh%2FVlZ7QKC5erDvxigo2NjabvepiLzwm4u1nwwHBXJMZFLRj80mlVlv5yHETi8%2Bd9nbGAZcLCi3BUhNJ6w%3D%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20220405T093801Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY6O6ANAYA%2F20220405%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=6e2cbd64c1622739d6c8ae16f97bed54e7607f8b15ddc11c897a322bf379d565&hash=5511db07a9d8a75c683db7447c043203f1844f94188b4a3a78c02beda66d2f37&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0925231217315412&tid=pdf-2b863cf5-540c-4f68-bb47-3ff1cb12e22f&sid=394f70e22be7f544cc997b55263f4af11993gxrqb&type=client)]/[[Code](https://www.kerenfu.top/sources/Neuro_demo.zip)] 
   76    |    IFC    |      TMM       |   2017   | Iterative Feedback Control Based Salient Object Segmentation | [[Paper](https://ieeexplore.ieee.org/abstract/document/8094951/)]/[Code] 
   77    |   CCRF    |      TMM       |   2017   | Saliency Detection by Fully Learning A Continuous Conditional Random Field | [[Paper](http://www.kerenfu.top/sources/C_CRF_Fu.pdf)]/[Code] 
   78    |   ELER    |      CVPR      |   2017   | What is and what is not a salient object? learning salient object detector by ensembling linear exemplar regressors | [[Paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Xia_What_Is_and_CVPR_2017_paper.pdf)]/[[Code](http://cvteam.net/projects/CVPR17-ELE/ELE.html)] 
   79    |   DIMD    |       PR       |   2017   | Diversity Induced Matrix Decomposition Model for salient object detection | [[Paper](https://www.sciencedirect.com/science/article/pii/S0031320317300122)]/[Code] 
   80    |   ProS    |       NC       |   2018   | Salient Object Detection via Proposal Selection              | [[Paper](https://www.sciencedirect.com/science/article/pii/S0925231218300754)]/[Code] 
   81    |    WMR    |       NC       |   2018   | Saliency detection via affinity graph learning and weighted manifold ranking | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0925231218307033)]/[[Code](https://pan.baidu.com/s/1NFboaeuuBph_QQGgXuIcaA)] 
   82    |   RCRR    |      TIP       |   2018   | Reversion correction and regularized random walk ranking for saliency detection | [[Paper](https://ses.library.usyd.edu.au/bitstream/handle/2123/20604/2017-j-cai-TIP2762422-YuchenYuan-10.1109%3ATIP.2017.2762422.pdf?sequence=2&isAllowed=y)]/[[Code](https://github.com/yuanyc06/rcrr)] 
   83    |   JLSE    |      TIP       |   2018   | Exemplar-aided Salient Object Detection via Joint Latent Space Embedding | [[Paper](https://drive.google.com/open?id=1Nm2au9gsbBikxpl0dK4ZY2P4YibTFasy)]/[Code] 
   84    |    WFD    |       PR       |   2018   | Water flow driven salient object detection at 180 fps        | [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S003132031730434X)]/[[Code](https://github.com/huangxm14-thu/SaliencyWater)] 
   85    |    FBQ    |     Access     |   2018   | Hypergraph Optimization for Salient Region Detection Based on Foreground and Background Queries | [[Paper](https://minerva-access.unimelb.edu.au/bitstream/handle/11343/227747/08356641.pdf)]/[Code] 
   86    |   FTOE    |      TMM       |   2019   | Salient Object Detection via Fuzzy Theory and Object-level Enhancement | [[Paper](https://ieeexplore.ieee.org/document/8375812)]/[Code] 
   87    |    KSR    |      TIP       |   2019   | Visual Saliency Detection via Kernelized Subspace Ranking with Active Learning | [[Paper](https://www.researchgate.net/publication/336424725_Visual_Saliency_Detection_via_Kernelized_Subspace_Ranking_With_Active_Learning)]/[[Code](https://github.com/jiayusun/KSR-AL)] 
   88    |    FCB    |      TIP       |   2019   | Exploiting Color Volume and Color Difference for Salient Region Detection | [[Paper](https://www.researchgate.net/publication/332834212_Exploiting_color_volume_and_color_difference_for_salient_region_detection)]/[[Code](https://github.com/liuguanghai009/FCB)] 
   89    |    TSG    |     TCSVT      |   2019   | Salient Object Detection Via Two-Stage Graphs                | [[Paper](https://ieeexplore.ieee.org/document/8332961)]/[Code] 
   90    |    DSC    |     TCSVT      |   2019   | Direction Selective Contour Detection for Salient Objects    | [[Paper](https://eprints.sztaki.hu/9808/1/Manno_375_3419087_ny.pdf)]/[Code] 
   91    |   AIGC    |     TCSVT      |   2019   | Adaptive Irregular Graph Construction Based Salient Object Detection | [[Paper](http://ieeexplore.ieee.org/document/8671726)]/[Code] 
   92    |    NIO    |     TNNLS      |   2019   | Semisupervised Learning Based on a Novel Iterative Optimization Model for Saliency Detection | [[Paper](https://ieeexplore.ieee.org/document/8378042)]/[Code] 
   93    |    MSR    |      TIP       |   2019   | 50 FPS Object-Level Saliency Detection via Maximally Stable Region | [[Paper](https://ieeexplore.ieee.org/document/8845759)]/[Code] 
   94    |   MSGC    |      TMM       |   2019   | Saliency Detection via Multi-Scale Global Cues               | [[Paper](https://cszjwang.github.io/sub_pages/pps/TMM19.pdf)]/[Code] 
   95    |    LRR    |      TIP       |   2019   | Local Regression Ranking for Saliency Detection              | [[Paper](https://ieeexplore.ieee.org/iel7/83/8835130/08850321.pdf)]/[Code] 






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
:triangular_flag_on_post: 15 | **IEEE TCyb** | Adjacent Context Coordination Network for Salient Object Detection in Optical Remote Sensing Images | [Paper](https://arxiv.org/pdf/2203.13664.pdf)/[Code](https://github.com/MathLee/ACCoNet) 





**No.** | **Name.** | **Pub.** | **Year** | **Title** | **Links** 
:-: | :-: | :-: | :-: | :-  | :-: 
01 | SuperCNN | IJCV | 2015 | A superpixelwise convolutional neural network for salient object detection | [Paper](https://link.springer.com/article/10.1007/s11263-015-0822-0)/[Code]
02 | LEGS | CVPR | 2015 | Deep networks for saliency detection via local estimation and global search | [Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Wang_Deep_Networks_for_2015_CVPR_paper.pdf)/[Code](https://github.com/huchuanlu/15_3)
03 | MC | CVPR | 2015 | Saliency detection by multi-context deep learning | [Paper](https://openaccess.thecvf.com/content_cvpr_2015/papers/Zhao_Saliency_Detection_by_2015_CVPR_paper.pdf)/[Code]
04 | MDF | CVPR | 2015 | Visual saliency based on multiscale deep features | [Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Li_Visual_Saliency_Based_2015_CVPR_paper.pdf)/[Code]
05 | DISC | TNNLS | 2016 | DISC: Deep image saliency computing via progressive representation learning | [Paper](https://ieeexplore.ieee.org/iel7/5962385/6104215/07372470.pdf)/[Code]
06 | DSL | TCSVT | 2016 | Dense and Sparse Labeling with Multi-Dimensional Features for Saliency Detection | [Paper](https://ieeexplore.ieee.org/iel7/76/4358651/07802636.pdf)/[Code]
07 | DS | TIP | 2016 | DeepSaliency: Multi-task deep neural network model for salient object detection | [Paper](https://ieeexplore.ieee.org/iel7/83/4358840/07488288.pdf)/[Code]
08 | SSD | ECCV | 2016 | A shape-based approach for salient object detection using deep learning | [Paper](https://link.springer.com/chapter/10.1007/978-3-319-46493-0_28)/[Code]
09 | CRPSD | ECCV | 2016 | Saliency Detection via Combining Region-Level and Pixel-Level Predictions with CNNs | [Paper](https://link.springer.com/chapter/10.1007/978-3-319-46484-8_49)/[Code]
10 | RFCN | ECCV | 2016 | Saliency detection with recurrent fully convolutional networks | [Paper](http://202.118.75.4/lu/Paper/ECCV2016/0865.pdf)/[Code](https://github.com/zengxianyu/RFCN)
11 | RFCN | TPAMI | 2019 | Salient object detection with recurrent fully convolutional networks | [Paper](https://ieeexplore.ieee.org/iel7/34/4359286/08382302.pdf)/[Code]
12 | MAP | CVPR | 2016 | Unconstrained salient object detection via proposal subset optimization | [Paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Zhang_Unconstrained_Salient_Object_CVPR_2016_paper.pdf)/[Code]
13 | SU | CVPR | 2016 | Saliency unified: A deep architecture for simultaneous eye fixation prediction and salient object segmentation | [Paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Kruthiventi_Saliency_Unified_A_CVPR_2016_paper.pdf)/[Code]
14 | RACDNN | CVPR | 2016 | Recurrent attentional networks for saliency detection | [Paper](https://openaccess.thecvf.com/content_cvpr_2016/papers/Kuen_Recurrent_Attentional_Networks_CVPR_2016_paper.pdf)/[Code]
15 | ELD | CVPR | 2016 | Deep Saliency with Encoded Low level Distance Map and High Level Features | [Paper](http://www.arxiv.org/pdf/1604.05495v1.pdf)/[Code](https://github.com/gylee1103/SaliencyELD)
16 | DHS | CVPR | 2016 | DHSNet: Deep Hierarchical Saliency Network for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Liu_DHSNet_Deep_Hierarchical_CVPR_2016_paper.pdf)/[Code](https://github.com/GuanWenlong/DHSNet-PyTorch)
17 | DCL | CVPR | 2016 | Deep Contrast Learning for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Li_Deep_Contrast_Learning_CVPR_2016_paper.pdf)/[Code]
18 | DSRCNN | ACMMM | 2016 | Deeply-Supervised Recurrent Convolutional Neural Network for Saliency Detection | [Paper](https://dl.acm.org/doi/pdf/10.1145/2964284.2967250)/[Code]
19 | MSCNet | ACMMM | 2017 | Multi-Scale Cascade Network for Salient Object Detection | [Paper](https://dl.acm.org/doi/pdf/10.1145/3123266.3123290)/[Code]
20 | CAR | BMVC | 2017 | Salient object detection using a context-aware refinement network | [Paper](http://www.cs.umanitoba.ca/~ywang/papers/bmvc17_detection.pdf)/[Code]
21 | DLS | CVPR | 2017 | Deep Level Sets for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Hu_Deep_Level_Sets_CVPR_2017_paper.pdf)/[Code]
22 | MSRNet | CVPR | 2017 | Instance-Level Salient Object Segmentation | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Li_Instance-Level_Salient_Object_CVPR_2017_paper.pdf)/[Code]
23 | WSS | CVPR | 2017 | Learning to Detect Salient Objects with Image-level Supervision | [Paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Wang_Learning_to_Detect_CVPR_2017_paper.pdf)/[Code](https://github.com/scott89/WSS)
24 | SRM | ICCV | 2017 | A stagewise refinement model for detecting salient objects in images | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Wang_A_Stagewise_Refinement_ICCV_2017_paper.pdf)/[Code](https://github.com/Pchank/caffe-sal)
25 | NLDF | CVPR | 2017 | Non-Local Deep Features for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Luo_Non-Local_Deep_Features_CVPR_2017_paper.pdf)/[Code](https://github.com/zhimingluo/NLDF)
26 | DSS | CVPR/TPAMI | 2017/2019 | Deeply Supervised Salient Object Detection with Short Connections | [Paper](http://arxiv.org/abs/1611.04849)/[Code](https://github.com/Andrew-Qibin/DSS)
27 | SalGAN | CVPR | 2017 | SalGAN: visual saliency prediction with adversarial networks | [Paper](http://arxiv.org/abs/1701.01081)/[Code](https://github.com/Pchank/caffe-sal)
28 | FSN | ICCV | 2017 | Look, perceive and segment: Finding the salient objects in images via two-stream fixation-semantic cnns | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Chen_Look_Perceive_and_ICCV_2017_paper.pdf)/[Code]
29 | DSOS | ICCV | 2017 | Delving into Salient Object Subitizing and Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/He_Delving_Into_Salient_ICCV_2017_paper.pdf)/[Code]
30 | SVF | ICCV | 2017 | Supervision by Fusion: Towards Unsupervised Learning of Deep Salient Object Detector  | [Paper](https://openaccess.thecvf.com/content_ICCV_2017/papers/Zhang_Supervision_by_Fusion_ICCV_2017_paper.pdf)/[Code](https://github.com/zhangyuygss/SVFSal.caffe)
31 | UCF | ICCV | 2017 | Learning Uncertain Convolutional Features for Accurate Saliency Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhang_Learning_Uncertain_Convolutional_ICCV_2017_paper.pdf)/[Code](https://github.com/Pchank/caffe-sal)
32 | AMU | ICCV | 2017 | Amulet: Aggregating Multi-level Convolutional Features for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhang_Amulet_Aggregating_Multi-Level_ICCV_2017_paper.pdf)/[Code](https://github.com/Pchank/caffe-sal)
33 | UGA | TIP | 2018 | An Unsupervised Game-Theoretic Approach to Saliency Detection | [Paper](https://pan.baidu.com/s/1U1O4oFK6ZALSghPjJv_5nA)/[Code](https://github.com/zengxianyu/uga)
34 | Refinet | TMM | 2018 | Refinet A deep segmentation assisted refinement network for salient object detection | [Paper](https://ieeexplore.ieee.org/iel7/6046/4456689/08419317.pdf)/[Code]
35 | MSED | Neurocomputing | 2018 | Multi-scale deep encoder-decoder network for salient object detection | [Paper](https://www.sciencedirect.com/science/article/pii/S0925231218308907)/[Code]
36 | EARNet | T-Cybernetics | 2018 | Embedding Attention and Residual Network for Accurate Salient Object Detection | [Paper](https://ieeexplore.ieee.org/iel7/6221036/9068331/08546752.pdf)/[Code]
37 | LFCS | T-Cybernetics | 2018 | Semi-Supervised Salient Object Detection Using a Linear Feedback Control System Model | [Paper](https://ieeexplore.ieee.org/iel7/6221036/6352949/08334814.pdf)/[Code]
38 | LICNN | AAAI | 2018 | Lateral inhibition-inspired convolutional neural network for visual attention and saliency detection | [Paper](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/viewFile/16230/16250)/[Code]
39 | ASMO | AAAI | 2018 | Weakly supervised salient object detection using image labels | [Paper](https://ojs.aaai.org/index.php/AAAI/article/download/12308/12167)/[Code]
40 | RADF | AAAI | 2018 | Recurrently aggregating deep features for salient object detection | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/12298/12157)/[Code]
41 | R3Net | IJCAI | 2018 | R3net: Recurrent residual refinement network for saliency detection | [Paper](https://www.ijcai.org/proceedings/2018/0095.pdf)/[Code]
42 | LFR | IJCAI | 2018 | Salient Object Detection by Lossless Feature Reflection | [Paper](https://pan.baidu.com/s/1DAyPHe_z0LJpKK8DxKF2dg)/[Code](https://github.com/Pchank/caffe-sal/blob/master/IIAU2018.md)
43 | C2SNet | ECCV | 2018 | Contour Knowledge Transfer for Salient Object Detection | [Paper](http://link-springer-com-s.vpn.whu.edu.cn:9440/content/pdf/10.1007/978-3-030-01267-0_22.pdf)/[Code](https://github.com/lixin666/C2SNet)
44 | RAS | ECCV | 2018 | Reverse Attention for Salient Object Detection | [Paper](http://arxiv.org/pdf/1807.09940)/[Code](https://github.com/ShuhanChen/RAS_ECCV18)
45 | LPSNet | CVPR | 2018 | Learning to promote saliency detectors | [Paper](https://pan.baidu.com/s/1QvDmqruH8oU51_GrgsuXoA)/[Code](https://github.com/zengxianyu/lps)
46 | RSOD | CVPR | 2018 | Revisiting salient object detection: Simultaneous detection, ranking, and subitizing of multiple salient objects | [Paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Islam_Revisiting_Salient_Object_CVPR_2018_paper.pdf)/[Code]
47 | DUS | CVPR | 2018 | Deep unsupervised saliency detection: A multiple noisy labeling perspective | [Paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Zhang_Deep_Unsupervised_Saliency_CVPR_2018_paper.pdf)/[Code](https://github.com/kris-singh/Deep-Unsupervised-Saliency-Detection)
48 | ASNet | CVPR | 2018 | Salient Object Detection Driven by Fixation Prediction | [Paper](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wang_Salient_Object_Detection_CVPR_2018_paper.pdf)/[Code](https://github.com/wenguanwang/ASNet)
49 | ASNet | TPAMI | 2019 | Inferring Salient Objects from Human Fixations | [Paper](https://ieeexplore.ieee.org/iel7/34/4359286/08668551.pdf)/[Code]
50 | BDMPM | CVPR | 2018 | A Bi-Directional Message Passing Model for Salient Object Detection | [Paper](https://pan.baidu.com/s/1akKVVipD8vIIv0XFrWND5Q)/[Code](https://github.com/zhangludl/A-bi-directional-message-passing-model-for-salient-object-detection) 
51 | DGRL | CVPR | 2018 | Detect Globally, Refine Locally: A Novel Approach to Saliency Detection | [Paper](https://pan.baidu.com/s/1ydLI0koPfndehqMOAwrK_Q)/[Code](https://github.com/TiantianWang/CVPR18_detect_globally_refine_locally) 
52 | PiCANet | CVPR | 2018 | PiCANet: Learning Pixel-wise Contextual Attention for Saliency Detection | [Paper](http://arxiv.org/abs/1708.06433)/[Code](https://github.com/Ugness/PiCANet-Implementation)
53 | PAGR | CVPR | 2018 | Progressive Attention Guided Recurrent Network for Salient Object Detection | [Paper](https://github.com/zhangxiaoning666/PAGR)/[Code](https://github.com/yangbinb/SalMetric/tree/master/PAGRN)
54 | DANet | JSTSP | 2019 | Distortion-adaptive Salient Object Detection in 360∘ Omnidirectional Images | [Paper](https://ieeexplore.ieee.org/iel7/4200690/5418892/08926489.pdf)/[Code]
55 | RSR | TPAMI | 2019 | Relative Saliency and Ranking: Models, Metrics, Data and Benchmarks | [Paper](https://ieeexplore.ieee.org/iel7/34/9280439/08756097.pdf)/[Code]
56 | Hyperfusion-Net | PR | 2019 | Hyperfusion-Net: Hyper-densely reflective feature fusion for salient object detection | [Paper](https://www.sciencedirect.com/science/article/pii/S0031320319301876)/[Code]
57 | Deepside | Neurocomputing | 2019 | Deepside: A General Deep Framework for Salient Object Detection | [Paper](https://www.sciencedirect.com/science/article/pii/S0925231219306484)/[Code]
58 | LVNet | TGRS | 2019 | Nested Network with Two-Stream Pyramid for Salient Object Detection in Optical Remote Sensing Images | [Paper](https://ieeexplore.ieee.org/iel7/36/8887423/08793227.pdf)/[Code]
59 | LFRWS | TIP | 2019 | Salient Object Detection with Lossless Feature Reflection and Weighted Structural Loss | [Paper](https://ieeexplore.ieee.org/iel7/83/4358840/08618369.pdf)/[Code]
60 | FBG | TIP | 2019 | Focal Boundary Guided Salient Object Detection | [Paper](https://ieeexplore.ieee.org/iel7/83/4358840/08603790.pdf)/[Code]
61 | ConnNet | TIP | 2019 | ConnNet: A long-range relation-aware pixel-connectivity network for salient segmentation | [Paper](https://ieeexplore.ieee.org/iel7/83/4358840/08576646.pdf)/[Code]
62 | CIG | TIP | 2019 | Deep Salient Object Detection with Contextual Information Guidance | [Paper](https://ieeexplore.ieee.org/iel7/83/4358840/08782147.pdf)/[Code]
63 | SPA | TIP | 2019 | Semantic Prior Analysis for Salient Object Detection | [Paper](https://ieeexplore.ieee.org/iel7/83/4358840/08624611.pdf)/[Code]
64 | CDMG | TIP | 2019 | Weakly Supervised Salient Object Detection by Learning A Classifier-Driven Map Generator | [Paper](https://ieeexplore.ieee.org/iel7/83/4358840/08720239.pdf)/[Code]
65 | CCAL | TMM | 2019 | Salient Object Detectioin Using Cascaded Convolutional Neural Networks and Adversarial Learning | [Paper](https://ieeexplore.ieee.org/iel7/6046/4456689/08649755.pdf)/[Code]
66 | SIA | TMM | 2019 | Saliency Integration An Arbitrator Model | [Paper](https://ieeexplore.ieee.org/iel7/6046/4456689/08411135.pdf)/[Code]
67 | MIJR | TCSVT | 2019 | Salient Object Detection via Multiple Instance Joint Re-Learning | [Paper](https://ieeexplore.ieee.org/iel7/6046/4456689/08768013.pdf)/[Code]
68 | AADF | TCSVT | 2019 | Aggregating Attentional Dilated Features for Salient Object | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8836095)/[Code](https://github.com/githubBingoChen/AADF-Net)
69 | ROSA | T-Cybernetics | 2019 | ROSA: Robust Salient Object Detection against Adversarial Attacks | [Paper](https://arxiv.org/pdf/1905.03434.pdf)/[Code](https://github.com/lhaof/ROSA-Robust-Salient-Object-Detection-Against-Adversarial-Attacks)
70 | SSNet | TPAMI | 2019 | Synthesizing Supervision for Learning Deep Saliency Network without Human Annotation | [Paper](https://ieeexplore.ieee.org/iel7/34/9108332/08645692.pdf)/[Code]
71 | DEF | AAAI | 2019 | Deep Embedding Features for Salient Object Detection | [Paper](https://pan.baidu.com/s/1HfyavmYB2NYUMe8CSe2qCw)/Code
72 | SuperVAE | AAAI | 2019 | Supervae: Superpixelwise variational autoencoder for salient object detection | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/4876/4749)/[Code]
73 | CapSal | CVPR | 2019 | CapSal: Leveraging Captioning to Boost Semantics for Salient Object Detection | [Paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_CapSal_Leveraging_Captioning_to_Boost_Semantics_for_Salient_Object_Detection_CVPR_2019_paper.pdf)/[Code](https://github.com/zhangludl/code-and-dataset-for-CapSal)
74 | BASNet | CVPR | 2019 | BASNet: Boundary Aware Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_CVPR_2019/html/Qin_BASNet_Boundary-Aware_Salient_Object_Detection_CVPR_2019_paper.html)/[Code](https://github.com/NathanUA/BASNet) 
75 | PFANet | CVPR | 2019 | Pyramid Feature Attention Network for Saliency detection | [Paper](https://arxiv.org/pdf/1903.00179.pdf)/[Code](https://github.com/CaitinZhao/cvpr2019_Pyramid-Feature-Attention-Network-for-Saliency-detection)
76 | MWS | CVPR | 2019 | Multi-source weak supervision for saliency detection | [Paper](https://arxiv.org/pdf/1904.00566.pdf)/[Code](https://github.com/zengxianyu/mws)
77 | ICNet | CVPR | 2019 | An Iterative and Cooperative Top-down and Bottom-up Inference Network for Salient Object Detection | [Paper](http://mftp.mmcheng.net/Papers/19cvprIterativeSOD.pdf)/Code
78 | PAGE-Net | CVPR | 2019 | Salient Object Detection With Pyramid Attention and Salient Edges | [Paper](https://www.researchgate.net/publication/332751907_Salient_Object_Detection_With_Pyramid_Attention_and_Salient_Edges)/[Code](https://github.com/wenguanwang/PAGE-Net)      
79 | CPD | CVPR | 2019 | Cascaded Partial Decoder for Accurate and Fast Salient Object Detection | [Paper](https://arxiv.org/pdf/1904.08739.pdf)/[Code](https://github.com/wuzhe71/CPD-CVPR2019)
80 | MLMSNet | CVPR | 2019 | A Mutual Learning Method for Salient Object Detection with intertwined Multi-Supervision | [Paper](https://pan.baidu.com/s/1EUxabfnEi_l5-ghUI3_qVQ)/[Code](https://github.com/JosephineRabbit/MLMSNet)
81 | AFNet | CVPR | 2019 | Attentive Feedback Network for Boundary-aware Salient Object Detection | [Paper](https://pan.baidu.com/s/1n-dRVC4sLWCmhhD5bnVXqg)/[Code](https://github.com/ArcherFMY/AFNet)  
82 | DPOR | ICCV | 2019 | Employing Deep Part-Object Relationships for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_Employing_Deep_Part-Object_Relationships_for_Salient_Object_Detection_ICCV_2019_paper.pdf)/Code
83 | SIBA | ICCV | 2019 | Selectivity or Invariance: Boundary-aware Salient Object Detection | [Paper](https://arxiv.org/pdf/1812.10066.pdf)/Code
84 | JDF | ICCV | 2019 | Structured Modeling of Joint Deep Feature and Prediction Refinement for Salient Object Detection | [Paper](https://arxiv.org/pdf/1909.04366.pdf)/[Code](https://github.com/xuyingyue/DeepUnifiedCRF_iccv19)
85 | FLoss | ICCV | 2019 | Optimizing the F-measure for Threshold-free Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhao_Optimizing_the_F-Measure_for_Threshold-Free_Salient_Object_Detection_ICCV_2019_paper.pdf)/[Code](https://github.com/zeakey/iccv2019-fmeasure)
86 | HRSOD | ICCV | 2019 | Towards High-Resolution Salient Object Detection | [Paper](https://arxiv.org/pdf/1908.07274.pdf)/[Code](https://github.com/yi94code/HRSOD)
87 | EGNet | ICCV | 2019 | EGNet: Edge Guidance Network for Salient Object Detection | [Paper](http://mftp.mmcheng.net/Papers/19ICCV_EGNetSOD.pdf)/[Code](https://github.com/JXingZhao/EGNet)
88 | SCRN | ICCV | 2019 | Stacked Cross Refinement Network for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Wu_Stacked_Cross_Refinement_Network_for_Edge-Aware_Salient_Object_Detection_ICCV_2019_paper.pdf)/[Code](https://github.com/wuzhe71/SCRN)
89 | PoolNet | ICCV | 2019 | A Simple Pooling-Based Design for Real-Time Salient Object Detection | [Paper](https://arxiv.org/pdf/1904.09569.pdf)/[Code](https://github.com/backseason/PoolNet) 
PoolNet: 
90 | DeepUSPS | NeurIPS | 2019 | Deep Robust Unsupervised Saliency Prediction With Self-Supervision | [Paper](https://arxiv.org/pdf/1909.13055.pdf)/[Code](https://drive.google.com/file/d/10GlmenXR7nEJyRlmPHouvHP-g9KfUW1F/view)   
91 | EAI | ICLR | 2019 | Efficient Saliency Maps for Explainable AI | [Paper](https://arxiv.org/pdf/1911.11293)/[Code]
54 | DFI | TIP | 2020 | Dynamic Feature Integration for Simultaneous Detection of Salient Object, Edge and Skeleton | [Paper](http://mftp.mmcheng.net/Papers/20TIP-DFI.pdf)/[Code](https://github.com/backseason/DFI)
55 | CALoss | TIP | 2020 | Contour-aware loss: Boundary-aware learning for salient object segmentation | [Paper](https://ieeexplore.ieee.org/iel7/83/9263394/09262030.pdf)/[Code]
54 | EGNL | TCSVT | 2020 | Edge-guided non-local fully convolutional network for salient object detection | [Paper](https://ieeexplore.ieee.org/iel7/76/4358651/09036909.pdf)/[Code]
54 | CAGNet | PR | 2020 | CAGNet: Content-aware guidance for salient object detection | [Paper](https://www.sciencedirect.com/science/article/pii/S0031320320301072)/[Code]
53 | CAGNet | TIP | 2020 | CAGNet: Content-Aware Guidance for Salient Object Detection | [Paper](https://arxiv.org/abs/1911.13168)/[Code](https://github.com/Mehrdad-Noori/CAGNet)
53 | FastSaliency | T-Cybernetics | 2020 | Lightweight Salient Object Detection via Hierarchical Visual Perception Learning | [Paper](https://ieeexplore.ieee.org/document/9285193)/[Code](https://github.com/yun-liu/FastSaliency)

91 | PFPNet | AAAI | 2020 | Progressive Feature Polishing Network for Salient Object Detection | [Paper](https://arxiv.org/pdf/1911.05942.pdf)/[Code](https://github.com/chenquan-cq/PFPN) 
53 | F3Net | AAAI | 2020 | F3Net: Fusion, Feedback and Focus for Salient Object Detection | [Paper](https://arxiv.org/pdf/1911.11445.pdf)/[Code](https://github.com/weijun88/F3Net)  
53 | GCPANet | AAAI | 2020 | Global Context-Aware Progressive Aggregation Network for Salient Object Detection | [Paper](https://github.com/JosephChenHub/GCPANet/blob/master/GCPANet.pdf)/[Code](https://github.com/JosephChenHub/GCPANet) 
53 | ADASOD | AAAI | 2020 | Multi-spectral Salient Object Detection by Adversarial Domain Adaptation | [Paper](https://cse.sc.edu/~songwang/document/aaai20b.pdf)/Code 
53 | MTSA | AAAI | 2020 | Multi-Type Self-Attention Guided Degraded Saliency Detection | [Paper](https://cse.sc.edu/~songwang/document/aaai20a.pdf)/Code
53 | ScrSOD | CVPR | 2020 | Weakly-Supervised Salient Object Detection via Scribble Annotations | [Paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_Weakly-Supervised_Salient_Object_Detection_via_Scribble_Annotations_CVPR_2020_paper.pdf)/[Code](https://github.com/JingZhang617/Scribble_Saliency)  
53 | MINet | CVPR | 2020 | Multi-scale Interactive Network for Salient Object Detection | [Paper](https://drive.google.com/file/d/1gUYu0hO_8Xc5jgpzetuOVFDrqeSOiKZN/view?usp=sharing)/[Code](https://github.com/lartpang/MINet)  
53 | ITSD | CVPR | 2020 | Interactive Two-Stream Decoder for Accurate and Fast Saliency Detection | [Paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Zhou_Interactive_Two-Stream_Decoder_for_Accurate_and_Fast_Saliency_Detection_CVPR_2020_paper.pdf)/[Code](https://github.com/moothes/ITSD-pytorch)  
53 | LDF | CVPR | 2020 | Label Decoupling Framework for Salient Object Detection | [Paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Wei_Label_Decoupling_Framework_for_Salient_Object_Detection_CVPR_2020_paper.pdf)/[Code](https://github.com/weijun88/LDF)  
53 | Sal100K | ECCV | 2020 | Highly Efficient Salient Object Detection with 100K Parameters | [Paper](http://mftp.mmcheng.net/Papers/20EccvSal100k.pdf)/[Code](https://github.com/MCG-NKU/Sal100K)
53 | NSOD | ECCV | 2020 | n-Reference Transfer Learning for Saliency Prediction | [Paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123530494.pdf)/[Code](https://github.com/luoyan407/n-reference)   
53 | ABP-Saliency | ECCV | 2020 | Learning Noise-Aware Encoder-Decoder from Noisy Labels by Alternating Back-Propagation for Saliency Detection | [Paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123620341.pdf)/[Code](https://github.com/JingZhang617/Noise-aware-ABP-Saliency) 
53 | GateNet | ECCV | 2020 | Suppress and Balance: A Simple Gated Network for Salient Object Detection | [Paper](https://arxiv.org/pdf/2007.08074.pdf)/[Code](https://github.com/Xiaoqi-Zhao-DLUT/GateNet-RGB-Saliency) 
53 | FewCSOD | NeurIPS | 2020 | Few-Cost Salient Object Detection with Adversarial-Paced Learning | [Paper](https://papers.nips.cc/paper/2020/file/8fc687aa152e8199fe9e73304d407bca-Paper.pdf)/[Code](https://papers.nips.cc/paper/2020/file/8fc687aa152e8199fe9e73304d407bca-Supplemental.zip)

53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
53 | xx | xxx | 2020 | xxx | [Paper](xxx)/[Code]
54 | DNA | T-Cybernetics | 2021 | DNA: Deeply supervised nonlinear aggregation for salient object detection | [Paper](xxx)/[Code]

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


