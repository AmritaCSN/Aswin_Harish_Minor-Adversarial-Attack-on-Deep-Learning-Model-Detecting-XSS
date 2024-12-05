# Aswin_Harish_Minor-Adversarial-Attack-on-Deep-Learning-Model-Detecting-XSS
## **Overview**  
Cross-Site Scripting (XSS) attacks remain a critical security threat in web applications, enabling malicious actors to inject harmful scripts into webpages viewed by other users. These attacks can compromise sensitive data, execute unauthorized actions, or even hijack user accounts.

In this project, we develop a machine learning-based approach to detect XSS payloads using a deep learning model. The aims is to weaken the classification of the XSS detection model such that adversarial samples are to be identified as benign and evades the detection model while maintaining the functionality of the XSS payload on the target application(DVWA).

However, conventional machine learning models often struggle to detect adversarial inputs crafted to deceive the model by subtly altering the original data. To address this, we explore the generation of adversarial XSS payloads through character-level perturbations, to evaluate the model's robustness. These adversarial payloads mimic real-world obfuscation techniques attackers use to bypass detection systems and ensuring functionality of payloads remain even after being adversarially perturbed.

The project also introduces an evaluation framework to assess the model's performance on both standard and adversarial payloads. Insights gained from these evaluations highlight the vulnerabilities of the detection model and underscore the importance of adversarial training in improving resilience .

-----
## **Key Features**  
- **Deep Learning Detection**: A character-level RNN model trained to classify payloads as malicious or non-malicious.
- **Adversarial Attack Generation**: Creation of adversarial XSS payloads using encoding based perturbation.
- **Model Evaluation**: Model performance is tested against both normal and adversarial payloads to assess robustness.
- **Performance Impact Analysis**: Identifying the impact of perturbation across Precision,Recall,F1-Score,Detection Rate,Accuracy and Escape Rate.

------
# **Setup Instructions**
## Prerequisites
Ensure you have the following installed:

- **Python**: Version 3.8 or higher(Ideally the latest Version 3.12)
- **TensorFlow**: Version 2.16 
## Required Libraries

Install the following libraries before running the project:

- **NumPy**  
- **Pandas**  
- **Scikit-learn**  
- **Matplotlib**  
- **Jupyter Notebook**  
- **VS Code Extensions**:
  - **Python** (for Python environment support)  
  - **Jupyter** (for running notebooks in VS Code)
--------
## Threat Model

Below is the threat model diagram for the project:

![Threat Model](/src/img/ThreatModel_final.jpg)
--------
## Dataset Used
- **XSS_Dataset.csv**:Compilation of Portswigger and OWASP XSS cheatsheet 

--------
## Files and Directories

- **src/**: Contains the dataset and related files
  - **XSS_Dataset.csv**: A CSV file containing XSS payloads and their corresponding labels (malicious or non-malicious).
  - **img/**: Directory containing project-related images
    - **ThreatModel_final.png**: A diagram illustrating the threat model.

- **code.ipynb**: A Jupyter Notebook that includes the full code implementation, including data preprocessing, model training, and adversarial sample generation.

- **README.md**: This file, containing the project documentation, including setup instructions, usage, and details about the model and adversarial attacks.

-------
