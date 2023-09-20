![test4](https://github.com/Smainfet/Smainfet/assets/97527246/1cd67f86-a83d-4153-a74d-f109a36f865d)

<h2 align="center">
  Hi 👋 I'm Smaïn, a fresh biomedical engineer 🩻 passionate about Deep learning
</h2>


- 💙 I've just finished my end-of-studies internship with Carmat
  
- 📖 I have just obtained my biomedical engineering diploma from the [University of Technology of Compiegne (UTC)](https://utc.fr)

- 🌱 At the moment, I'm learning about deep learning techniques specifically for medical image processing
  
- 📫 Feel free to contact me on [LinkedIn](https://www.linkedin.com/in/sma%C3%AFn-fettem-55865917b/)
  
<br />
<br />


<h2>
  🗂️ My projects 
</h2>


For a better comprehension, here is a legend to contextualize my projects :

- 🔒 : Professional project, the code cannot be shown

- 📚 : Educational project
  
- 🩻 : Image processing project
  
- 〰️ : Signal processing project
  
- 🦾 : Robotics project

---
<h3>
  📚 🩻 Automatic Segmentation of CT images of lungs affected by COVID-19
</h3>

As part of the course _Medical image processing_, i developed a solution to perform an automatic segmentation of lungs affected by COVID-19.


Due to the scale of people affected by Covid-19 and because the scanners have great inter-variability, I proposed a robust and rapid lung segmentation method, using Deep Learning U-Net architecture, which will serve as a pre-processing step of a **hypothetic** chain of automatic diagnosis, to focus the automatic analysis of the CT scan images on the lung region.

<div align="center">
<img width="596" alt="Capture d’écran 2023-09-20 à 11 45 41" src="https://github.com/Smainfet/Smainfet/assets/97527246/03de4915-ecc7-4570-8ef0-e0d6697db765">

 

| <img width="400" alt="Capture d’écran 2023-09-20 à 13 09 17" src="https://github.com/Smainfet/Smainfet/assets/97527246/c35d4073-47ae-456e-a22f-d8333788fe90"> | 
|:--:| 
| <sub><sup> *comparison of segmentation results obtained with several methods* </sup></sub>|

</div>

I used [data available on kaggle](https://www.kaggle.com/datasets/andrewmvd/covid19-ct-scans) labeled by expert in segmentation. To improve training, I removed the volumes where there were no lungs.
<br />

<p align="center">
<img width="693" alt="Capture d’écran 2023-09-20 à 02 56 57" class="center" src="https://github.com/Smainfet/Smainfet/assets/97527246/be5e62eb-146c-4543-b2d2-f0c861ae05b6">
</p>


We can imagine that this processing chain will be used to direct health services as quickly and reliably as possible towards the diagnosis of the patient observed, and thus relieve them of this workload.

<h3>
  📚 〰️ Automatic Segmentation of CT images of lungs affected by COVID-19é
</h3>

An experimental study was carried out on 74 subjects recorded in two states: an initial state of relaxation followed by a phase of stress where the subject performs different stressful tasks (mental calculation, stroop test which is a color game). 

Four physiological signals including: ECG, PPG, EDA and EMG are recorded during both phases. As part of this work, I worked on PPG signal preprocessing. I developed a processing chain including: Exploratory data analysis, PPG signal processing and extraction of temporal, frequency and statistical parameters.

At the same time, I worked on an interface capable of reproducing signal acquisition and applying filtering in real time.
