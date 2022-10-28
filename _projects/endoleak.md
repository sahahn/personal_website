---
date: 2018-12-1
published: true
title: "Automated Endoleak and AAA Detection"
description: "Automated Detection and Segmentation of Endoleaks and Abdominal Aortic Aneurysm"
project_tags: python, Medical Imaging, Deep Learning, Research
media: Website
ownership:
time_period: Summer 2018 - Spring 2019
thumbnail: "/projects/endoleak/predictleak.gif"

website:
  button_text: See the framework developed for this project
  url: https://github.com/sahahn/GenDiagFramework

intro: |
  This project represents more of a series of incremental projects that I worked on starting in the Summer of 2018 up until Spring 2019. This
  project represented a new collaboration between the Complex Systems Center, which I has just joined as a Master's student in
  [Safwan Wshah's lab](https://swshah.w3.uvm.edu/vail/group.php), and the UVM medical center. On the UVM medical center end of things, I worked mainly
  with two excellent doctors, vascular surgeon [Daniel Bertges](https://www.uvmhealth.org/medcenter/provider/daniel-j-bertges-md) and interventional radiologist
  [Christopher Morris](https://www.uvmhealth.org/medcenter/provider/christopher-s-morris-md).

  The goal of this project was to build from the ground up a comprehensive set of tools to assist, in an automated way, in various tasks related to the pathology around Abdominal Aortic Aneurysm (AAA) patient care. In particular, we developed tools to first isolate a smaller region of interest around the AAA, perform EndoLeak detection and lastly 3D segmentation of the Aneurysm itself (providing automated measurements of AAA volume). The input to all of these tools was computed tomography angiography (CTA) imaging from a collection of patients who underwent care at the University of Vermont Medical center.

  This project was made both more interesting and difficult in that no pre-existing labelled dataset existed. In this way it differs greatly from simmilar projects on prepared public datasets for say the prediction of lung cancer. In this project we instead had to work from the level of coarse natural text labelling that existing as saved in the UVM medical center. We were therefore required to build the deep learning system through a series of creative semi-automated labelling schemes, as well as semi-automated text mining tools. In particular, sparse 3D labelling was used for the by far most intenstive piece (3D dense segmentation of AAA).
  
  A paper on this work ["Machine deep learning accurately detects endoleak after endovascular abdominal aortic aneurysm repair"](https://www.sciencedirect.com/science/article/pii/S2666350319300045) was published in JVS-Vascular Science. This paper recieved the 2020 JVS most viewed article award. This work was also presented as a keynote presentation at the 2019 Vascular Annual Meeting of the Society for Vascular Surgery, National Harbor, Md, June 12-15, 2019. An earlier, more methods focused, paper [Deep Learning for Recognition of Endoleak After Endovascular Abdominal Aortic Aneurysm Repair](https://ieeexplore.ieee.org/abstract/document/8759187) was published and presented as a poster at the 2019 IEEE 16th International Symposium on Biomedical Imaging (ISBI 2019). Lastly, this worked was filled in US Patent Application No.: 17/602,164 Title: METHOD AND APPARATUS FOR ANALYZING AORTIC ANEURYSMS AND ENDOLEAKS IN COMPUTED TOMOGRAPHY SCANS.

  Due to various difficulties related to patient privacy, only a generalized subset of the code is avaliable for this project on [github](https://github.com/sahahn/GenDiagFramework).


content_layout:

  - section_layout: 2col

    videos:

      - caption: Full slideshow presenting research project and results
        description: Slides
        url: https://docs.google.com/presentation/d/e/2PACX-1vTOwAlpRKR9wzGyfo_-T5jusAmO3VH9jwx8VhWRrI6U-yTO9JFrpNVX8MxAf8GCriTg9uILiz96bcDW/embed?start=false&loop=false&delayms=5000

    images:

      - caption: Overview of the pipeline illustrating use of three modified convolutional neural networks (CNNs). See "Machine deep learning accurately detects endoleak after endovascular abdominal aortic aneurysm repair" for a more detailed description of the full algorithm.
        description: 'Full final project workflow'
        url: '/projects/endoleak/pipe.jpg'
        width:
        height:

      - caption: Example showing a view of how multi-class sparse segmentation was performed per patient's scan, where 3-5 slices in each dimension were labelled. Green=EndoGraft, Red=AAA. This process of sparse segmentation saves a huge amount of manual effort, and still contains enough information for the 3D segmentation network to learn. Essentially, the network predicts in 3 dimensionals, but the loss function will only score on labeled pieces. 
        description: Example sparse 3D segmentation
        url: '/projects/endoleak/sparse_seg.gif'
        width:
        height:

      - caption: This gif shows example predictions from a 2D CNN trained to perform binary classification on axial CT images to predict for the presence or absence of an EndoLeak on that slice. Eventually, predictions are combined across all slices, as well as across imaging contrasts, into a single binary prediction  representing the probability the patient exhibits an EndoLeak.
        description: 'Predict EndoLeak per Slice'
        url: '/projects/endoleak/predictleak.gif'
        width:
        height:

      - caption: Results on a single scan from the trained 3D CNN for automated multi-class segmentation, Red is predicted AAA, Green is predicted EndoGraft. In practice, these results were used internally to generate new ground truth segmentations by 'fixing' the mistakes of the network when predicting on new subjects. 
        description: 'Automated multi-class segmentation, Red is AAA, Green is EndoLeak.'
        url: '/projects/endoleak/predict_seg.gif'
        width:
        height:

   

---
