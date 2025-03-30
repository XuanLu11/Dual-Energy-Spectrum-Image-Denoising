# Dual-Energy-Spectrum-Image-Denoising
Correction Practice of Dual-Energy Spectrum Images

## Project Overview  
Medical imaging devices collect **dual-energy data**, which is processed using conventional methods to generate **basis images**. These basis images correspond to different material compositions of the same tissue. This process can be represented as:  

$\[
\left( d_1, d_2 \right) \rightarrow (f, g)
\]$

where $\( d_1, d_2 \)$ denote the dual-energy data, and $(f, g)$ are the generated basis images. The arrow **"→"** represents a conventional data processing method. However, since $\( d_1 \)$ and $\( d_2 \)$ contain noise, and traditional methods often have **local limitations**, the generated basis images $(f, g)$ may deviate significantly from the true images $(f^{*}, g^{*})$.  

### Task Objective  
This project aims to enhance the generated images $(f, g)$ using deep learning methods so that they become closer to the true images $(f^*, g^*)$, while also improving generalization on the test set.  

The task can be viewed as a denoising problem, where the true images $(f^*, g^*)$ are corrupted by unknown noise. The goal is to learn the characteristics of this noise using deep learning techniques and improve the quality of the reconstructed images.  
