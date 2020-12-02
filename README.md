# Mid-SURE-2019
## Automatic Segmentation of Pediatric Chest Radiographs with Deep Learning
### Greg Holste

<img src="Figs/FinalHolsteMidSure.jpg" width=500 height=500 class="center">

Repository for *Automatic Segmentation of Pediatric Chest Radiographs with Deep Learning*, a poster presented at ![Mid-SURE 2019](https://urca.msu.edu/files/forums/36/booklet/2019%20Mid-SURE%20Program%20Book%20-%20Digital.pdf) on July 24, 2019. This work (in progress at the time) was conducted at the ![ACRES REU](https://icer-acres.msu.edu/) under Dr. Adam Alessio at Michigan State University.

Here you can find the poster presented (`FinalHolsteMidSURE.pdf`) and an auxiliary notebook (`results.ipynb`) showing more detailed segmentation results.

---

**Abstract**: Patients in neonatal and pediatric intensive care units often require catheters and tubes, collectively referred to as "lines," to sustain life. These patients undergo a series of chest radiographs throughout their stay to ensure proper line placement, and each study must be assessed by a radiologist, representing a time-consuming, labor-intensive process. Here we employ deep learning approaches to automate line monitoring by segmenting the chest into medically relevant regions, locating lines, and determining whether each line is appropriately placed relative to those regions. In an IRB-approved study, pediatric chest radiographs were collected and annotated with custom software in which users drew boundaries around seven regions of the chest: left and right lung, left and right subdiaphragm, spine, mediastinum, and carina. We trained a U-Net, a type of fully convolutional neural network for biomedical image segmentation, implemented in Keras on 240 chest radiographs and their binary masks. On a test set of 43 radiographs, our model achieved 92.3% mean pixel accuracy and a mean Dice coefficient of 0.768. Qualitatively, the model produces realistic predictions for large regions like the lungs and spine. However, in some cases, boundaries between regions are unrealistic and, most crucially, the carina – the small point at which the trachea splits into each bronchus – is never correctly classified. Work is ongoing to implement weighted loss functions to overcome these challenges. At present, this approach offers an initial step toward the goal of providing automatic, anatomic context for line placement assessment.
