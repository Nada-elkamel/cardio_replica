# 🫀 CardioReplica

**CardioReplica** is a deep learning and digital twin project for cardiovascular data analysis, cardiac modeling, and biventricular digital twin generation.

The project is implemented through **Kaggle Jupyter notebooks** using **Python, PyTorch, and TensorFlow**, and is organized into five main phases, progressing from cardiovascular data processing and model development to **3D/4D digital twin generation and interactive visualization**.

## 📊 Dataset

The project uses the **EchoNext v1.1.0** dataset from **PhysioNet**.

The dataset provides the basis for the experiments and analyses performed throughout the different phases of the project.

## 🧰 Technologies

* 🐍 **Python**
* 🔥 **PyTorch**
* 🧠 **TensorFlow**
* 📓 **Jupyter Notebooks**
* 📊 **Kaggle**
* 🏥 **PhysioNet**
* 🧊 **PyVista 0.42.3**
* 🔬 **VTK 9.3.0**
* 🫀 **3D/4D Digital Twin**
* 📈 **Interactive Dashboard**

## 🔬 Project Pipeline

CardioReplica is organized into **five phases**, covering the complete workflow from data-driven cardiac analysis to digital twin generation.

### Phase 1 — Data Preparation

The first phase focuses on preparing the cardiovascular data for subsequent analysis and modeling.

It includes the processing and organization of the available data to create suitable inputs for the machine learning and deep learning experiments.

### Phase 2 — Deep Learning

The second phase focuses on developing deep learning models using **PyTorch** and **TensorFlow**.

The notebooks provide the implementation and experimentation environment for training and evaluating the developed models on the cardiovascular data.

### Phase 3 — Cardiac Analysis and Modeling

The third phase focuses on cardiac-related analysis and modeling based on the processed data and the outputs of the previous stages.

The objective is to extract meaningful information that can contribute to the reconstruction and representation of cardiac anatomy and motion.

### Phase 4 — 3D Cardiac Representation

The fourth phase extends the analysis toward a three-dimensional representation of the heart.

This phase prepares the cardiac geometry and the information required for the generation of the biventricular digital twin.

### Phase 5 — 3D/4D Digital Twin Generation and Dashboard

The fifth phase focuses on the generation, deformation, rendering, and visualization of the biventricular digital twin.

The digital twin generation relies on **PyVista 0.42.3**, a high-level Python interface to **VTK 9.3.0**, for constructing, deforming, and rendering the biventricular mesh derived from the **UKBRVLV atlas**.

PyVista applies the bounded PCA-based shape deformations (Section ??) and exports the resulting end-diastole to end-systole motion sequence as **T = 30 binary `.vtp` surface mesh frames**, which are compiled into animated GIFs for visual inspection outside full 3D rendering environments.

A dedicated **dashboard** is also provided to facilitate the visualization and exploration of the generated digital twins. The dashboard provides an interactive interface for inspecting the reconstructed biventricular geometry, deformation sequence, and cardiac motion results.

This final phase therefore provides an accessible way to explore the generated **3D/4D cardiac digital twin** and its temporal evolution.

## 🫀 Digital Twin

The final output of the pipeline is a **biventricular cardiac digital twin** representing the transition from **end-diastole to end-systole**.

The 4D representation consists of a temporal sequence of **30 `.vtp` surface mesh frames**, allowing the cardiac geometry and deformation to be inspected throughout the simulated cardiac motion.

The generated meshes can be rendered and visualized using the PyVista/VTK pipeline and inspected through the project dashboard.

## 📊 Dashboard

The CardioReplica dashboard provides an interactive visualization layer for the generated digital twins.

It is designed to facilitate:

* 🫀 Visualization of the biventricular cardiac geometry
* 🔄 Exploration of the end-diastole to end-systole motion sequence
* 📐 Inspection of 3D cardiac mesh deformation
* 🎞️ Visualization of the temporal 4D sequence
* 📊 Exploration of the generated digital twin results

The dashboard complements the Kaggle notebooks by providing a more accessible interface for inspecting the generated cardiac models and their motion.
<img width="1915" height="905" alt="Capture d&#39;écran 2026-08-23 202108" src="https://github.com/user-attachments/assets/14a06bf5-f984-4329-be15-c1dec1040edb" />

## 📓 Repository Structure

```text
cardio_replica/
│
├── *.ipynb
│
└── README.md
```

The repository is primarily composed of **Python/Kaggle Jupyter notebooks** containing the different phases of the CardioReplica pipeline.

## ▶️ Running the Project

The notebooks are designed to be used in the **Kaggle environment**.

To reproduce the experiments:

1. Open the required notebook in Kaggle.
2. Make the required **EchoNext v1.1.0** dataset available.
3. Run the notebook cells sequentially.
4. Generate and inspect the corresponding outputs.
5. For the final phase, use the generated cardiac meshes and visualization pipeline to explore the 3D/4D digital twin and dashboard.

## 📦 Main Outputs

Depending on the phase, the project produces:

* Processed cardiovascular data
* Deep learning models and results
* Cardiac analysis outputs
* 3D biventricular representations
* `.vtp` surface mesh files
* A sequence of **30 cardiac motion frames**
* Animated visualizations
* 3D/4D digital twin representations
* Interactive dashboard visualizations

## 🎯 Project Objective

The main objective of **CardioReplica** is to explore the use of **artificial intelligence, deep learning, 3D modeling, and digital twin technologies** for cardiovascular applications.

The project combines data-driven approaches with anatomical modeling to move from cardiovascular data and learned representations toward an interactive **3D/4D biventricular cardiac digital twin**.

## ⚠️ Disclaimer

CardioReplica is intended for **research and educational purposes**.

The models, visualizations, and results generated by this project should not be considered a substitute for professional medical diagnosis, treatment, or clinical decision-making.

## 👩‍💻 Author

**Nada El Kamel**

GitHub: **Nada-elkamel**
