# An LLM-Enabled-Multimodal-Agentic-AI Framework for the Medical Internet of Things MIoT
Integration of large language models (LLM) with multimodal agentic artificial intelligence (AI) within the medical Internet of Things (MIoT) ecosystem

Authors detail:  M. A. RAHMAN∗, College of Computer and Cyber Sciences, University of Prince Mugrin, Madina, KSA
SYED USMAN JAMIL, School of Computing, Mathematics and Engineering, Charles Sturt University, Wagga
Wagga NSW, Australia
M SHAMIM HOSSAIN, Department of Software Engineering, College of Computer and Information Sciences,
King Saud University, KSA
MUHAMMAD ARIF KHAN, School of Computing, Mathematics and Engineering, Charles Sturt University, Wagga
Wagga NSW, Australia
TANVEER ZIA, School of Arts and Sciences, University of Notre Dame, NSW, Australia
MUHAMMAD ALI PARACHA, CDC, Melbourne, Australia
MUBARAK ALRASHOUD, Department of Software Engineering, College of Computer and Information Sciences,
King Saud University, KSA
MIN CHEN, School of Computer Science and Engineering, South China University of Technology, China
SELWA AL-HAZZAA, Digital Innovation Sector, King Abdulaziz City for Science and Technology (KACST), KSA

**Introduction**

This repository explores the integration of Large Language Models (LLMs) and multimodal, agentic AI within the Medical Internet of Things (MIoT), a synergy that is fundamentally reshaping modern healthcare. By combining diverse data streams, this approach enables continuous patient monitoring, adaptive clinical decision support, and intelligent, context-aware human-machine collaboration.
Healthcare environments produce vast amounts of multimodal data: text from electronic health records (EHRs) and clinical notes; medical scans like MRI, CT, and X-rays; audio from patient consultations; video for therapy monitoring; and real-time sensor data such as ECG and glucose levels. Traditional single-mode AI struggles to interpret this complex ecosystem. In contrast, LLM-augmented agentic systems excel at fusing these varied sources, grounding their reasoning in medical knowledge, and orchestrating specialized agents to improve real-world clinical operations.
We provide a comprehensive guide to LLM-driven multimodal agentic AI for MIoT healthcare systems. The core of this work is a six-dimensional unified taxonomy covering:
•	Multimodal Input Channels
•	Data Fusion Techniques
•	Core LLM Reasoning Abilities
•	Agent Coordination Models
•	Computational Deployment Layers
•	Ethical Governance Frameworks

To illustrate this framework in practice, we include a detailed Virtual Hospital case study focused on oncology. This study demonstrates how intelligent agents integrate multimodal signals such as medical images, genomic data, patient conversations, and clinical updates to deliver personalized diagnostics, automate documentation, support home-based rehabilitation, and facilitate rapid emergency response.

**Contact** 📬: If you want to contribute, you can contact:  [Syed Usman Jamil](usmanjamilsyed@gmail.com) 📧 Prof. M SHAMIM HOSSAIN

**Contributions:**

A novel taxonomy that structures multimodal agentic AI powered by LLM in MIoT healthcare across six layers:

Layer 1: Input multimedia streams

Layer 2: Fusion strategies

Layer 3: LLM roles 

Layer 4: Agentic and multi-agent coordination

Layer 5: Deployment architectures

Layer 6: Governance/compliance

**Datasets and Benchmarks:** Publicly Available MIoT and multimodal healthcare datasets and highlits of benchmark initiatives

| Category | Dataset | Key Modalities | Primary Application |
|:---|:---|:---|:---|
| **Physiological Signals** | MIMIC-IV [1] | ECG, Vitals, Labs, Clinical Notes | Critical Care Monitoring & Analysis |
| | PhysioNet Databases | ECG, EEG, EMG, PPG | General Physiological Signal Research |
| | WESAD | Multi-sensor (ECG, EDA, ACC) | Stress & Affect Recognition |
| **Medical Imaging** | NIH ChestX-ray14 [2], CheXpert | Chest Radiographs (X-rays) | Thoracic Pathology Detection |
| | LIDC-IDRI | Lung CT Scans | Lung Nodule & Cancer Detection |
| | EyePACS, Messidor | Retinal Fundus Images | Diabetic Retinopathy Screening |
| | HAM10000 | Dermoscopy Images | Skin Lesion Classification |
| **Audio & Speech** | IEMOCAP [3] | Speech, Video, Text | Emotion Recognition (Clinical PROMs) |
| | COUGHVID | Cough Audio Recordings | Respiratory Disease Analysis |
| | PhysioNet Auscultation | Heart & Lung Sounds | Cardiovascular/Pulmonary Monitoring |
| **Video & Action** | UTD-MHAD [4] | RGB Video, Depth, Inertial Sensors | Human Activity Recognition |
| | UP-Fall Detection | Video, Accelerometer | Fall Detection & Prevention |
| | MM-Fit | Video, IMU Data | Rehabilitation Exercise Monitoring |
| **Textual Data (EHR)** | MIMIC-IV Notes [5] | Clinical Notes (Discharge, Nursing) | Clinical NLP & Information Extraction |
| | i2b2 2014 | Annotated Clinical Narratives | De-identification & Privacy Research |
| | n2c2 Shared Tasks | Discharge Summaries | Medication, Relation, & Temporal NLP |
| **Multimodal Composite** | Med-VQA Datasets [6] | Medical Images + Text QA | Visual Question Answering |
| | AVEC Series | Audio, Video, Text | Multimodal Affect Recognition |
| | BioVid Heat Pain | Physiological Signals + Video | Pain Estimation & Analysis |

| Benchmark | Modalities | Primary Focus | Current Limitation |
|:---|:---|:---|:---|
| **MedVidQA** | Video + Text | Medical instructional video question answering | Limited to procedural QA; lacks clinical workflow integration. |
| **VQA-RAD** | Radiology Images + Text | Visual question answering for radiology images | Focused on single-image QA; no multi-step agent orchestration. |
| **MultiMedQA (Google)** | Text + (Planned Multimodal) | Evaluating large medical LLM knowledge & reasoning | Primarily textual; multimodal queries are nascent. |
| **BioNLP Shared Tasks** | Text + Biomedical KBs | Biomedical knowledge integration & relation extraction | Lacks multimodal grounding in sensor/imaging data. |
| **AVEC Challenges** | Audio + Video + Physiology | Multimodal affect & behavioral analysis | Not yet adapted for clinical decision-support workflows. |

Identified Research Gaps
⚠️ Critical Gap: No existing benchmark fully addresses multi-agent orchestration or complex medical cyber-physical (MCP) aligned workflows. This highlights an urgent need for new benchmarks that:

⚠️ Evaluate coordinated multi-agent systems across modalities.

⚠️ Simulate real-world clinical workflows and interventions.

⚠️ Integrate live sensor data with static medical records and images.

⚠️ Require sequential decision-making and task decomposition across specialized AI agents.


## **Security Threats and Defenses for LLM-Based Healthcare AI**

### **Introduction to Threat Modeling**
Effectively securing LLM-based healthcare pipelines requires a proactive **threat modeling** approach. This involves identifying potential adversaries—from malicious external actors to curious insiders with varying system access—and their capabilities as a foundational step for building robust defenses. Frameworks like **STRIDE**, adapted for LLMs in healthcare, provide a structured methodology for this analysis.

| Threat Category | Description & Mechanism | Healthcare-Specific Example | Reference / Framework |
| :--- | :--- | :--- | :--- |
| **Threat Modeling** | Systematic identification of vulnerabilities in LLM-based healthcare pipelines, considering adversaries with different access levels. | Applying adapted STRIDE methodology to assess risks in a diagnostic agent system. | STRIDE for LLMs in Healthcare|
| **Adversarial Examples** | Malicious, often imperceptible, perturbations added to input data (images, audio, sensor readings) to cause model misclassification. | Altered radiology scans leading to incorrect diagnosis; manipulated IoT vital sign data. | NIST AI 100-2e Taxonomy |
| **Prompt Injection Attacks** | Crafted inputs designed to hijack the LLM's behavior, bypass safety guards, or extract sensitive data from the model. | Hidden instructions embedded within a patient's uploaded image or clinical note text. | OWASP Top 10 LLM Risks [5], Multimodal Injection Cases |
| **Data Poisoning** | Insertion of corrupted or biased data during the model's training phase to degrade its performance or introduce backdoors. | Introducing fraudulent sensor logs in a federated learning network for patient monitoring. | NIST Adversarial Machine Learning Report |
| **Model Inversion / Membership Inference** | Attacks that attempt to reconstruct training data or determine if a specific individual's data was part of the training set. | Querying a medical LLM to infer the presence of a celebrity's health records in its training data. | Privacy Attacks in NIST AI 100-2e |
| **LLM-Driven Physical Misbehavior** | Exploitation of LLMs controlling physical devices (robots, IoT actuators) to execute harmful or unintended actions. | Using a malicious prompt to instruct a surgical assistive robot to perform an unsafe maneuver. | RoboPAIR Security Study  |
| **Defense: Adversarial Training** | Training models on a mixture of clean and adversarially perturbed data to improve robustness against evasion attacks. | Implementing this technique within federated learning pipelines for healthcare to protect distributed models. | DHS/DoD Adversarial AI Mitigations |
| **Defense: Secure Deployment** | Implementing rigorous security practices including ISO 27001-aligned audits, penetration testing, and continuous monitoring. | Integrating these controls within a Healthcare Information Security Management System (ISMS) for AI deployment. | RSNA AI Security Review |


**Acknowledgments**

We thank all collaborators and institutions contributing datasets, insights, and clinical expertise that informed this
repository.

**References**

[1] Johnson, A., et al. MIMIC-IV. PhysioNet (2023). Access: https://physionet.org/content/mimiciv/3.1/

[2] Wang, X., et al. ChestX-ray8. CVPR (2017). Access: https://www.kaggle.com/datasets/nih-chest-xrays/data

[3] Busso, C., et al. IEMOCAP. Speech Communication (2008). Access:	https://sail.usc.edu/iemocap/

[4] Chen, C., et al. UTD-MHAD. CVPRW (2015). Access: https://personal.utdallas.edu/~kehtar/UTD-MHAD.html

[5] Johnson, A., et al. MIMIC-IV-Note. Nature Scientific Data (2023). Access: https://www.physionet.org/content/mimic-iv-note/2.2/

[6] Lau, J., et al. Med-VQA. Medical Image Analysis (2018). Access: https://www.med-vqa.com/




