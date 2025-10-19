This project analyzes the **Robot Execution Failures Dataset** from the UCI Machine Learning Repository.The dataset contains **force and torque measurements** recorded from a robot after various failure events. Using the power of **IBM Granite (Granite 3.3-8B Instruct)** running in **Google Colab**, this project performs:
- Data reading and parsing of robotic logs
- Automatic summarization per failure type
- Insight extraction and pattern detection
- Visualization and final reporting in PDF

This project demonstrates how **AI-driven analysis** can be used to interpret complex robotic sensor data and produce meaningful insights that can guide system improvement and reliability optimization.

---

##  Key operational events

    1. Common failure types
    2. Root cause patterns
    3. Recommended corrective actions

The project combines Summarization (to compress log data into actionable insights) and Mini Classification (to categorize detected failure patterns).

## Raw Dataset
**Source:** [UCI Machine Learning Repository – Robot Execution Failures](https://archive.ics.uci.edu/dataset/83/robot+execution+failures)

- `lp1.data` → Failure in approach to grasp position  
- `lp2.data` → Failure in transfer of a part  
- `lp3.data` → Positioning failure after transfer  
- `lp4.data` → Failure in approach to ungrasp position  
- `lp5.data` → Failure in motion with part

Each file contains **15 force/torque samples** recorded at regular time intervals.

---

## Technical Stack

| Technical | Tools |
|------|--------------|
| AI Model | IBM Granite 3.3-8B Instruct |
| Platform | Google Colab |
| Integration | Replicate API |
| Language | Python |
| Libraries | langchain_community, replicate, pandas, matplotlib |

##  Analysis Process
1. **Data Upload & Reading**  
   All five `.data` files were read and processed using Python in Colab.  

2. **IBM Granite Summarization**  
   For each dataset, IBM Granite generated a summary that includes:
   - Main operational phases  
   - Detected anomalies or abnormal readings  
   - Possible causes of failures  
   - Recommendations for improvement  

3. **Result Aggregation**  
   All summaries were combined into one cohesive report using IBM Granite again.

4. **Visualization**  
   A keyword frequency and pie chart were created to identify dominant error categories such as `collision`, `sensor`, `torque`, and `obstruction`.
## Analysis Process
1. **Data Upload & Reading**  
   All five `.data` files were read and processed using Python in Colab.  

2. **IBM Granite Summarization**  
   For each dataset, IBM Granite generated a summary that includes:
   - Main operational phases  
   - Detected anomalies or abnormal readings  
   - Possible causes of failures  
   - Recommendations for improvement  

3. **Result Aggregation**  
   All summaries were combined into one cohesive report using IBM Granite again.

4. **Visualization**  
   A keyword frequency and pie chart were created to identify dominant error categories such as `collision`, `sensor`, `torque`, and `obstruction`.

---

## Insight & Findings
| Key Aspect | Description |
|-------------|-------------|
| **Dominant Failures** | Most common anomalies were `sensor errors` and `collisions`, representing more than 60% of total findings. |
| **Root Causes** | Torque imbalance, poor sensor calibration, and workspace obstructions were identified as major contributors. |
| **Environmental Impact** | Uneven terrain or magnetic interference likely influenced force/torque readings. |
| **Mechanical Issues** | Repeated patterns in left/right torque suggest alignment and drive system instability. |

---

## Recommendations
1. Recalibrate all robotic sensors to reduce signal drift.  
2. Optimize path planning algorithms to minimize collision risk.  
3. Expand workspace clearance and add dynamic obstacle detection.  
4. Conduct regular maintenance to prevent torque overload and mechanical fatigue.  
5. Integrate AI-driven anomaly detection for continuous monitoring.

---

## Visualization
The following chart shows the overall distribution of dominant keywords detected by IBM Granite across all datasets:

![IBM Granite Error Keywords](ibm_granite_piechart.png)

**Top Error Categories**
- Sensor-related anomalies → 31.8%  
- Collision issues → 31.8%  
- Obstruction & calibration → 27.2% combined  

---

##  AI Support Explanation
IBM Granite was responsible for:
- Reading and understanding raw robotic logs  
- Summarizing each dataset independently  
- Detecting patterns and anomalies  
- Generating a unified analytical report  
- Producing natural language recommendations  

---

## Key Outputs
| File | Description |
|------|-------------|
| `summary_lp1.data.txt` → `summary_lp5.data.txt` | IBM Granite’s individual dataset summaries |
| `final_robot_report.txt` | Combined insights from all summaries |
| `ibm_granite_piechart.png` | Visualization of keyword distribution |
| `IBM_Granite_Robotic_Report.pdf` | Final professional report (ready to print & submit) |

---

## Conclusion
Through IBM Granite’s AI capabilities, the robot’s operational data was successfully transformed into actionable insights.  
The project demonstrates that **AI can serve as an analytical co-pilot** for robotics engineers  identifying errors, predicting failure causes, and proposing improvements autonomously.

---

##  Author

Name:  CyberTech(Nata)  
Program: AI & Robotics  
Platform: Hacktiv8 – Capstone Project 
Model Used: IBM Granite 3.3-8B Instruct  
Year: 2025  

---

##  Notes
This project is designed according to **Hacktiv8 Capstone Submission Requirements**, including:
- GitHub Repository  
- Google Colab Notebook  
- README Documentation  
- Visualization

---

## Dataset License & Attribution

**Dataset Source:**  
[Robot Execution Failures Dataset – UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/83/robot+execution+failures)  
Donated by: **Luis Montesano**, **Juan Manuel Blanco**, **Manuel Lopes**, and **Manuel T. de la Torre**  
Date: April 22, 1999  

**License:**  
This dataset is made publicly available by the UCI Machine Learning Repository for research and educational purposes.  
You are free to use, modify, and distribute the dataset, provided that proper attribution is given to the original authors and source.

**Citation (recommended):**  

