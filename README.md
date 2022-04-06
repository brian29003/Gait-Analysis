# Gait-Analysis
2D computer vision and OpenPose pose estimation for gait analysis

<img src='https://github.com/brian29003/Gait-Analysis/blob/main/demo.gif?raw=true'>

**Background**:

Gait analysis refers to the study of the walking posture of patients. Gait analysis could be used by physiotherapist to diagnose pathological motion, plan treatment and monitor physiotherapy outcomes. 

Clinical gait analysis requires clinical set-up including motion capture markers, ground reaction force measuring mats. Alternatively, the gait of patients could be analyzed by experienced therapists.

During pandemic, tele-rehabilitation is getting popular. If the gait of patients could be captured by pose estimation using deep learning, and extract some of the “gait parameters” or even the “gait health index”, the patients may have some ideas on the progress of recovery. Furthermore, the nursing home can use this technology to help the elderies to monitor their health without high cost. 

This project is based on the idea research of Kidziński[1], and further explore the potential of using LSTM and CNN-LSTM to improve model performance. And also using the model to test on new data.

**Objective**

With the use of neural network, predict the "healthiness" of patients' gaits with given gait videos. First use OpenPose to obtain time series of joint position in videos. Then train a deep learning model with the dataset that labelled the gait video with clinical assessment result, GDI.

**Reference**:

[1] Ł. Kidziński, B. Yang, J. L. Hicks, A. Rajagopal, S. L. Delp, and M. H. Schwartz, “Deep neural networks enable quantitative movement analysis using single-camera videos,” Nat Commun, vol. 11, no. 1, p. 4054, Dec. 2020, doi: 10.1038/s41467-020-17807-z.

In our project, we will be using the same dataset, but we will try exploring other deep learning methods and compare the results. Also, we will try to use the model on a small new dataset

**Dataset**:

Available:https://simtk.org/projects/video-gaitlab. The dataset was released in the research mentioned before

The dataset includes the position of joints in gait analysis. The position are obtained by pose estimation software OpenPose (https://github.com/CMU-Perceptual-Computing-Lab/openpose). The videos were taken while performing clinical gait analysis.
