# DDos-Detection-Using-Machine-Learning-Algorithms-Python

In today's digital landscape, where connectivity and reliance on online services are paramount, the threat posed by cyberattacks has reached unprecedented levels. Among these threats, Distributed Denial of Service (DDoS) attacks stand out as a significant concern for organizations and individuals alike. These attacks can disrupt the availability of critical online services, causing substantial financial losses and reputational damage. To combat this evolving threat, the integration of machine learning algorithms for DDoS attack detection has emerged as a promising avenue.

At its core, a Denial of Service (DoS) attack involves overwhelming a target system, such as a web server or network, with an excessive volume of requests, rendering the system inaccessible to legitimate users. This form of attack exploits the finite resources of the targeted system, causing temporary unavailability. In contrast, a Distributed Denial of Service (DDoS) attack takes this malevolent strategy to a new level. By orchestrating a network of compromised devices, the attacker magnifies their impact, creating a surge of malicious traffic that can overpower even robust infrastructure.

In the realm of network security, the detection and mitigation of Distributed Denial of Service (DDoS) attacks represent a pivotal challenge. Conventional approaches relying on rule-based and signature-based methods are proving inadequate in the face of evolving attack strategies. Their rigidity hinders adaptation to emergent attack patterns, resulting in elevated rates of false positives and a deficiency in real-time responsiveness. The requisite manual intervention exacerbates the issue, culminating in delayed detection and response times.

The project "DDoS Detection using Machine Learning" focuses on developing an advanced system to effectively detect and classify Distributed Denial of Service (DDoS) attacks within network traffic. The project employs various machine learning algorithms including Logistic Regression, Support Vector Machine (SVM), Random Forest, and Gradient Boosting, and evaluates their performance against a dataset of network traffic features. The dataset is extensively analyzed and visualized to understand its characteristics. Each model is trained, optimized, and rigorously tested to determine its accuracy, precision, recall, and F1-score. The outcomes highlight the superiority of the Random Forest model with a perfect accuracy of 100%, while SVM and Gradient Boosting also demonstrate robust performance. The study emphasizes the significance of comprehensive evaluation metrics in selecting the optimal model for DDoS detection in real-world network security scenarios.

## Objectives 
- Data Collection and Pre-processing: Source a comprehensive and representative dataset containing instances of normal network traffic as well as various types of DDoS attacks. Pre-process and cleanse the data to ensure consistency and reliability for subsequent analysis.

- Algorithm Selection and Implementation: Delve into the landscape of machine learning algorithms and choose those that are well-suited for binary classification tasks. For this project, we explore the applicability of Logistic Regression, Support Vector Machine (SVM), Random Forest, and Gradient Boosting techniques.


- Model Training and Evaluation: Employ the chosen algorithms to train predictive models using the pre-processed data. Evaluate the models' performance using a suite of evaluation metrics, including accuracy, precision, recall, and F1-score.

- Comparative Analysis: Perform an in-depth comparative analysis of the implemented algorithms' effectiveness in detecting DDoS attacks. Understand the trade-offs between different algorithms in terms of accuracy, efficiency, and adaptability to varying attack scenarios.


- Reduced False Positives: Design algorithms that minimize false positive rates by discerning between legitimate traffic fluctuations and genuine DDoS attacks. Achieving a higher level of accuracy will alleviate the unnecessary strain on resources caused by false alarms.

## Flowchart
![image](https://github.com/Abhirambs-08/DDos-Detection-Using-Machine-Learning-Algorithms-Python/assets/119886477/86b78255-13bd-48b8-bc52-c61976eb8876)


## Testing and Validation
### Performing DDoS and its testing
A Distributed Denial of Service (DDoS) attack is a malicious attempt to disrupt the normal functioning of a target website or online service by overwhelming it with a massive volume of traffic from multiple sources. Kali Linux is a popular penetration testing and ethical hacking platform that provides various tools for assessing and testing the security of networks and systems. One such tool is GoldenEye, a Python-based application used to launch DDoS attacks. Wireshark, on the other hand, is a widely used network protocol analyzer that captures and inspects network traffic in real-time. Here is a description of how to perform a DDoS attack using GoldenEye and capture the data using Wireshark:

- Performing the DDoS Attack using GoldenEye:

  - Setup Kali Linux: Ensure that you have Kali Linux installed on your system or a virtual machine.

  - Install GoldenEye: Open a terminal and use the package manager to install GoldenEye

  - Choose a Target: Identify the target website you want to perform the DDoS attack on. This could be a site you own and have permission to test, or you can use a public testing site with permission.

  - Launch the Attack: Run GoldenEye from the terminal with the target website's URL as an argument. You can also specify other options like the number of threads and duration of the attack. GoldenEye will start sending a flood of requests to the target server, overwhelming its resources and potentially causing it to become unresponsive.

- Capturing Data in Wireshark:
  
  - Start Wireshark: Open Wireshark by typing wireshark in the terminal.

  - Choose Capture Interface: Select the network interface through which the DDoS attack traffic will be sent and received. This could be your Ethernet interface or Wi-Fi adapter.

  - Start Capturing: Click the "Start" button in Wireshark to begin capturing network traffic on the selected interface.

  - Analyze Captured Data: As the DDoS attack is ongoing, Wireshark will capture and display the network packets in real-time. You can analyze the captured data to see the flood of requests being sent to the target server and the responses it generates.

  - Save Captured Data: Once you have captured enough data to analyze, you can stop the capture and save the captured packets to a file for further examination.
![image](https://github.com/Abhirambs-08/DDos-Detection-Using-Machine-Learning-Algorithms-Python/assets/119886477/1a475cf7-734e-43d7-85c8-085b60b7e015)
![image](https://github.com/Abhirambs-08/DDos-Detection-Using-Machine-Learning-Algorithms-Python/assets/119886477/9102474d-4033-4bfd-b06c-0dae7250d014)

## RESULTS
Summary of the accuracy and performance metrics achieved by each model:

- Logistic Regression:
  - Accuracy: 76.64%
  - Best solver: liblinear
  -	Precision, recall, and F1-score are reported for both classes (0: Benign, 1: Malicious).
  - The model performs reasonably well, with good precision and recall for both classes.
- Support Vector Machine (SVM):
  - Accuracy: 97.0%
  - Best kernel: rbf
  - Similar to Logistic Regression, precision, recall, and F1-score are reported for both classes.
  - SVM shows high accuracy and balanced precision and recall for both classes.
- Random Forest:
  - Accuracy: 100.0%
  - The model achieves a perfect accuracy of 100%, indicating strong classification performance.
  - High precision, recall, and F1-score values are observed for both classes.
- Gradient Boosting:
  - Accuracy: 99.54%
  - The model shows excellent accuracy and balanced performance in terms of precision and recall. 
  - Both classes are well classified, indicating the effectiveness of Gradient Boosting.
    
These results showcase the capabilities of the trained models in accurately classifying network traffic as either benign or malicious. The Random Forest model stands out with its perfect accuracy, while other models like SVM and Gradient Boosting also demonstrate impressive performance. The choice of the best model should consider not only accuracy but also precision, recall, and F1-score, depending on the specific requirements of the DDoS detection system.
![image](https://github.com/Abhirambs-08/DDos-Detection-Using-Machine-Learning-Algorithms-Python/assets/119886477/fcd8c03b-e7fb-4970-85ee-2ae1525beba3)
![image](https://github.com/Abhirambs-08/DDos-Detection-Using-Machine-Learning-Algorithms-Python/assets/119886477/77b80dd9-8683-47f9-9984-7b00e1384606)


![image](https://github.com/Abhirambs-08/DDos-Detection-Using-Machine-Learning-Algorithms-Python/assets/119886477/b21b6e4c-43f5-47e5-940b-3302974e1a6a)

