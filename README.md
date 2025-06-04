# HypereSphereDiff: Harmonizing-Geometry-and-Uncertainty-Diffusion-with-Hyperspheres **[ICML 2025]**

![collage_page-0001](https://github.com/IAB-IITJ/Harmonizing-Geometry-and-Uncertainty-Diffusion-with-Hyperspheres/blob/main/static/SAFARI_IMAGES/vis_abs.png)
## Abstract
_Do contemporary diffusion models preserve the class geometry of hyperspherical data?_ Standard diffusion models rely on isotropic Gaussian noise in the forward process, inherently favoring Euclidean spaces. However, many real-world problems involve non-Euclidean distributions, such as hyperspherical manifolds, where class-specific patterns are governed by angular geometry within hypercones. When modeled in Euclidean space, these angular subtleties are lost, leading to suboptimal generative performance. To address this limitation, we introduce **HyperesphereDiff** to align hyperspherical structures with directional noise, preserving class geometry and effectively capturing angular uncertainty. Both theoretically and empirically, we demonstrate that this approach aligns the generative process with the intrinsic geometry of hyperspherical data, resulting in more accurate and geometry-aware generative models. We evaluate our framework on four object datasets and two face datasets, showing that incorporating angular uncertainty better preserves the underlying hyperspherical manifold.

## Contributions
The key contributions of our work are as follows:
- **Introduce a Class-Specific Hypercone Formalism:** We define class hypercones to preserve intra-class angular concentration while ensuring inter-class separation on the hypersphere.
- **Design a vMF-Based Forward and Reverse Process:** A novel dual-stream approach combining Whisper and m-HuBERT encoders with an Audio Feature Unification Module and large language model integration, designed specifically for multilingual deepfake detection.
- **Enable Diverse and Hard Sample Generation:** Unlike Gaussian noise, our vMF-based approach avoids simplicity bias, producing a well-spread distribution with challenging yet realistic samples. We introduce two metrics, Hypercone Coverage Ratio (HCR) and Hypercone Difficulty Skew (HDS) to assess distribution spread and sample difficulty.
- **Develop Theoretical Foundations and Empirical Evaluations:** We validate our approach with experiments, demonstrating improved alignment with intrinsic geometry and robustness to varying degrees of uncertainty in class-conditional tasks on 4 object datasets (CIFAR-10, MNIST, CUB-200, Cars-196) and 2 face datasets (CelebA, D-LORD).

## Proposed vMF based Diffusion Modeling

Forward vMF Diffusion             |  Reverse vMF Diffusion 
:-------------------------:|:-------------------------:
![](https://github.com/IAB-IITJ/Harmonizing-Geometry-and-Uncertainty-Diffusion-with-Hyperspheres/blob/main/static/SAFARI_IMAGES/2.gif) |  ![](https://github.com/IAB-IITJ/Harmonizing-Geometry-and-Uncertainty-Diffusion-with-Hyperspheres/blob/main/static/SAFARI_IMAGES/3.gif)


### Code coming soon...



