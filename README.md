
# DA-SFTFormer: Discrepancy-Aware and Spatial Feature Transform Former For Pixel-level Surface Defect Detection

Pixel-level surface defect detection aims to accurately locate defect regions, which is of great significance in industrial manufacturing quality inspection and intelligent infrastructure inspection. However, surface defects are often characterized by weak saliency, irregular boundaries, elongated structures, and high similarity to complex backgrounds, making accurate segmentation still highly challenging. Existing methods have two main shortcomings: first, direct multi-scale feature aggregation easily blurs the true structural boundaries and propagates background interference; second, static or insufficiently adaptive prediction mechanisms struggle to effectively model the significantly varying defect morphology and scene context between different samples. To address these issues, this paper proposes DA-SFTFormer for pixel-level surface defect detection. Specifically, we first design a Boundary-Aware Semantic Fusion (BASF) module, utilizing cross-scale response inconsistency as an implicit structural prior to enhance boundary-sensitive feature aggregation capabilities. Subsequently, we introduce a Spatial Feature Transformation (SFT) mechanism, which performs semantic-conditional affine modulation on high-resolution representations, preserving fine spatial structures while enhancing semantic consistency. Furthermore, we employ a Dynamic Context Query (DCQ) strategy to adaptively adjust query representations based on the global context of the current input image, thereby enhancing the modeling ability for different defect appearance patterns. Finally, we construct a Gated Edge-Enhanced Segmentation Head (GEES-Head), selectively injecting high-frequency boundary information while suppressing false boundary noise to further improve prediction quality. Extensive experiments demonstrate that DA-SFTFormer achieves superior performance on publicly available surface defect detection datasets, validating the effectiveness of this method in balancing semantic discriminativity, structural fidelity, and adaptive decoding capabilities in complex scenarios.

---

###  ⚠️ Notice
Remember to modify the path to the dataset before running the test and training code. Different image resolutions require modifying the relevant parameter parameters.


## 🙏 Acknowledgment 

Our project is based on **[WPFormer](https: //github.com/yfhdm/WPFormer)**, and we are very grateful for their excellent work. Their contributions laid the foundation for the development of our query-based defect detection technology.
