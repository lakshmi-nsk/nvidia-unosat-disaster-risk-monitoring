# Disaster Risk Monitoring Using Satellite Imagery

---

## Credits & Acknowledgements

I extend sincere gratitude to **[NVIDIA Corporation](https://www.nvidia.com/)** and the **[NVIDIA Deep Learning Institute (DLI)](https://www.nvidia.com/en-us/deep-learning-ai/education/)** for developing and providing the *Disaster Risk Monitoring Using Satellite Imagery* educational program, along with its laboratory materials. This curriculum has been instrumental in advancing my understanding of **GeoAI applications in disaster management**.

This repository draws upon Jupyter notebooks and resources from NVIDIA's program, created in collaboration with the **[United Nations Institute for Training and Research (UNITAR)](https://unitar.org/)** and the **[United Nations Satellite Centre (UNOSAT)](https://www.unitar.org/unosat)**. These materials are proprietary and restricted to enrolled participants.

> [!NOTE]
> The notebooks and code herein represent an **independent adaptation** for educational and research purposes, incorporating original analyses, enhanced visualizations, and extensions developed by the author.

> [!IMPORTANT]
> No proprietary NVIDIA code, confidential datasets, or restricted resources are included in this repository.

---

## Overview

This repository presents an **advanced adaptation** of NVIDIA DLI's program, illustrating the application of **deep learning** and **geospatial analytics** to delineate and evaluate natural disaster impacts using satellite observations.

![Flood Visualization](https://d32xksboxpocwt.cloudfront.net/shrine_store/uploads/networks/263/ne_events/3410/wide-4b29978db8eb6a6c4f2ce76db8272116.webp)

Through hands-on experimentation with **Sentinel-1 Synthetic Aperture Radar (SAR) imagery**, this work employs **segmentation models** and **visualization tools** to construct a robust pipeline for flood risk assessment—extensible to landslides, wildfires, and other environmental hazards.

Emphasizing independent scholarly extensions, the repository integrates:  

- Enhanced visualizations  
- Analytical augmentations  
- Fine-tuning via the **[NVIDIA Train, Adapt, Optimize (TAO) Toolkit)](https://developer.nvidia.com/tao-toolkit)**

This effort bridges **Artificial Intelligence (AI)**, **satellite remote sensing**, and **disaster resilience**, advancing **GeoAI**—the fusion of AI with geospatial sciences.

*Aligned with the United Nations Sustainable Development Goals (SDGs), this project contributes to:*  

1. **SDG 6: Clean Water and Sanitation** – Assessing flood impacts on water resources and sanitation systems.  
2. **SDG 9: Industry, Innovation, and Infrastructure** – Deploying innovative technologies for resilient infrastructure.  
3. **SDG 11: Sustainable Cities and Communities** – Informing risk-based urban development.  
4. **SDG 13: Climate Action** – Enabling data-informed strategies for disaster mitigation and adaptation.

---

## Description

This repository encapsulates an **educational and research-oriented adaptation** of a flood risk monitoring pipeline, leveraging satellite imagery, deep learning, and geospatial visualization.

### Key Components

1. **Satellite Data Processing**  
   - Handling **Sentinel-1 SAR imagery** for flood delineation via noise mitigation, thresholding, and temporal change detection.

2. **Deep Learning-Based Image Segmentation**  
   - Deploying the **U-Net architecture** for pixel-level classification of flooded regions, with fine-tuning via **[NVIDIA TAO Toolkit](https://developer.nvidia.com/tao-toolkit)**.

3. **Geospatial Visualization**  
   - Generating mapped outputs using **[Basemap](https://matplotlib.org/basemap/)** and **[Matplotlib](https://matplotlib.org/)** for spatial interpretation and overlay on administrative features.

4. **Case Study Application**  
   - Focused on flood detection, with extensibility to landslides, wildfires, or droughts.

> [!NOTE]
> Integrates principles from **computer vision**, **supervised learning**, **data engineering**, and **remote sensing**, prioritizing **ethical data handling** and **responsible AI** in humanitarian contexts.

---

## Features

- **Flood Detection from Sentinel-1 SAR Imagery**  
  - Detects flood extents under adverse conditions (e.g., cloud cover), ensuring operational reliability where optical data fails.

- **Deep Learning with U-Net Architecture and NVIDIA TAO Toolkit**  
  - Semantic segmentation of pixels as flooded or non-flooded.  
  - Efficient adaptation using **transfer learning** and **GPU optimization**.

- **Geospatial Visualization and Map Overlays**  
  - Provides interpretable visualizations for disaster responders, planners, and humanitarian agencies.

---

## Technologies and Models Used

### Programming Libraries & Tools

- `NumPy` – Numerical computations and array operations.  
- `Pillow` – Image manipulation.  
- `Matplotlib` – Visualization and plotting.  
- `Jupyter Notebook` – Interactive prototyping.  
- `Triton Client (HTTP)` – Interface with **[NVIDIA Triton Inference Server](https://developer.nvidia.com/nvidia-triton-inference-server)**.

### Model Architectures

- `U-Net` – Semantic segmentation for flood mapping.  
- `SSD-512`, `RetinaNet`, `YOLOv3` – Object detection for damaged infrastructure or fire hotspots.

### NVIDIA Tools & Frameworks

- `TAO Toolkit` – Streamlines transfer learning for vision models.  
- `TensorRT` – Optimizes inference performance.  
- `Triton Inference Server` – Scalable, real-time model serving.

### Data & Preprocessing

- **Satellite Imagery** – [Sentinel-1](https://scihub.copernicus.eu/), [Sentinel-2](https://scihub.copernicus.eu/), [GOES](https://www.goes.noaa.gov/), [VIIRS](https://ncc.nesdis.noaa.gov/viirs/)  
- **Geographic Information Systems (GIS)** – Fuse satellite data with spatial layers for hazard mapping.

### Deep Learning Applications

- **Image Classification** – Land cover classification (water, burned areas).  
- **Object Detection** – Detecting damaged buildings or active fires.  
- **Semantic Segmentation** – Delineating disaster zones at pixel resolution.

---

## Usage Instructions

1. **Enroll in the Learning Program:** [Disaster Risk Monitoring Using Satellite Imagery - NVIDIA DLI](https://courses.nvidia.com/courses/course-v1:DLI+S-ES-01+V1)  
2. **Launch the Cloud Lab Environment:** Access a pre-configured GPU-enabled workspace.  
3. **Locate the Notebooks:** Navigate to the `notebooks/` directory.  
4. **Open the First Notebook:** Launch the notebook containing the “NGC API Setup” cell.  
5. **Authenticate with NGC:** Execute the setup cell using your [NGC API key](https://ngc.nvidia.com).  
6. **Automatic Resource Download:** NGC CLI fetches models, datasets, and containers.  
7. **Begin Analysis:** Proceed to data processing, model training, and visualization.

---

## References & Links

- **[Disaster Risk Monitoring Using Satellite Imagery – NVIDIA DLI Course Portal](https://courses.nvidia.com/courses/course-v1:DLI+S-ES-01+V1)**  
- **[NVIDIA Blog: UN Satellite Centre Boosts SDGs](https://blogs.nvidia.com/blog/un-satellite-centre-boosts-sustainable-development-goals/)**  
- **[UNOSAT Knowledge Hub Event](https://knowledgehub.unosat.org/events/3410)**  
- **[NGC Developer Portal](https://ngc.nvidia.com/)**  
