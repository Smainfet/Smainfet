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


<h1>
  🗂️ My projects 
</h1>


For a better comprehension, here is a legend to contextualize my projects :

- 🔒 : Professional project, the code cannot be shown

- 📚 : Educational project
  
- 🩻 : Image processing project
  
- 〰️ : Signal processing project
  
- 🦾 : Robotics project


<h2>
  📚 🩻 Automatic Segmentation of CT images of lungs affected by COVID-19
</h2>

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

<h2>
  📚 〰️ Preprocessing of a PPG signal for stress identification and visualization interface
</h2>


An experimental study was carried out on 74 subjects recorded in two states: an initial state of relaxation followed by a phase of stress where the subject performs different stressful tasks (mental calculation, stroop test which is a color game). Four physiological signals including: ECG, PPG, EDA and EMG are recorded during both phases. 


As part of this work, I worked on PPG signal preprocessing. I developed a processing chain including: Exploratory data analysis, PPG signal processing and extraction of temporal, frequency and statistical parameters.

<div align="center">
<img width="600" alt="Capture d’écran 2023-09-20 à 23 20 32" src="https://github.com/Smainfet/Smainfet/assets/97527246/e5d5ee74-1735-45e1-9c3b-8f18def94166">
</div>

At the same time, I worked on a PyQt5 interface capable of reproducing signal acquisition and applying filtering in real time.

<div align="center">
  
![ezgif com-optimize-2](https://github.com/Smainfet/Smainfet/assets/97527246/d88b68ef-fd39-45f6-8a71-f3ea4d9d0b68)

</div>

<h2>
  🔒 🩻 MR‐based treatment planning in radiotherapy using deep learning approach
</h2>
<div align="center">
<img width="650" alt="image" src="https://github.com/Smainfet/Smainfet/assets/97527246/b82d8757-c194-418c-8e71-92f8e72c7cdb">
</div>

In radiotherapy, MRI is used for target volume and organs-at-risk delineation for its superior soft-tissue contrast as compared to CT imaging. However, MRI does not provide the electron density of tissue necessary for dose calculation. Several methods of synthetic-CT (sCT) generation from MRI data have been developed for radiotherapy dose calculation. 

My work was to test, propose and upgrade different deep learning (DL) sCT generation methods, in order to improve results obtains on the associated image created with the DL method, in the context of MRI-based dose calculation.

I proposed a new cGAN (Conditional generative adversarial network) method based on the 3 MRI image views (transverse, sagittal and coronal) and not only on the axial view (like classic cGAN method).

<div align="center">
<img width="600" alt="Capture d’écran 2023-09-20 à 23 44 50" src="https://github.com/Smainfet/Smainfet/assets/97527246/b18bf922-e862-4b5d-bc1b-57bd7bd4c651">
</div>

The 2D+ cGAN (cGAN in the 3 views) consists of generating 3 sCTs (according to each view) per patient, and combined in one sCT by using the median voxel value. 

The biggest problem I encountered was the presence of artifacts in the final sCTs. Artifacts were created upstream of the final sCT, by the sCTs generated on the x and y axis. A lack of space outside the patient's external contour during the testing phase corrupts the generation of the sCT. I concluded that the generator does not have a wide enough intensity dynamic in the MRI to synthesize the sCT correctly, this causes it to confuse the low values of the MRI inside the outer contour ( 20 - 30 intensity) for outdoors (0 intensity).

I was able to obtain one of the best result of the literature for sCT generation in the pelvis area.

<div align="center">
  
| <img width="500" alt="image" src="https://github.com/Smainfet/Smainfet/assets/97527246/2204d1bf-0f75-4074-abbc-6e4dc53b71e3">|<img width="300" alt="Capture d’écran 2023-09-21 à 00 26 44" src="https://github.com/Smainfet/Smainfet/assets/97527246/bad1bffb-d34c-48db-9d68-321441355f41">|
|   :----:    |    :----:   |

</div>

[This 2D+ method was published at the ESTRO (European Society Radiation Oncology) 2022 congress.](https://www.estro.org/Congresses/ESTRO-2022/665/imagingacquisitionandprocessing/11217/evaluationofsynthetic-ctgeneratedfromprostatemri-0)


