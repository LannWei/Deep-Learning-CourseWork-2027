# Deep Learning Final Project 2026/27 – Tactile Perception

In this project you will train deep learning models on images from a **GelSight
vision-based tactile sensor**. There are two tasks:

- **Shape classification:** recognise which of 10 shapes is pressed into the sensor.
- **Force estimation:** predict the 3D contact force (`fx`, `fy`, `fz`, in newtons),
  including the tangential (shear) components.

The assessment has two parts. **Part A** is a technical report (60%) and **Part B** is a
video presentation (40%).

---

## Files

| File | Contents |
|---|---|
| **[`Tactile_DL_2027.zip`](https://github.com/LannWei/Deep-Learning-CourseWork-2027/releases/latest/download/Tactile_DL_2027.zip)** (on the [Releases](https://github.com/LannWei/Deep-Learning-CourseWork-2027/releases) page) | Dataset (~37 MB), dataset README, and an example submission |
| [`2027_Final_Project_Assessment.pdf`](2027_Final_Project_Assessment.pdf) | Assessment slides: tasks and marking criteria for Part A and Part B |
| [`2027_Deep_Learning_Report_Guidance.pdf`](2027_Deep_Learning_Report_Guidance.pdf) | Report guidance: objectives and steps for each task, and deliverables |

**Start by reading `README.md` inside the zip.** It explains:

- the data format and labels
- how to load the data in Google Colab
- how to split the data
- the required evaluation metrics
- the exact submission interface for your models

---

## Assessment overview

### Part A – Report (60%)

| Task | Points |
|---|---|
| Task 1: Data preparation and preprocessing | 10 (+2 bonus) |
| Task 2: Shape classification | 20 (+4 bonus) |
| Task 3: Force estimation (regression) | 20 (+4 bonus) |
| Task 4: Hyperparameter tuning (optional) | up to 5 bonus |
| Task 5: Report writing and visualisation quality | 10 |

Your trained models will also be run on a **hidden test set** that is not released.

### Part B – Video presentation (40%)

Present a creative deep learning solution to a stakeholder challenge. Marks are awarded
for:

- problem and stakeholder introduction (10)
- proposed solution overview (10)
- novelty (10)
- presentation quality (10)

See `2027_Final_Project_Assessment.pdf` for the full criteria.

---

## Getting started

1. Get the dataset. The zip is too large for the repository itself, so it is attached to
   the [**Releases**](https://github.com/LannWei/Deep-Learning-CourseWork-2027/releases)
   page.
   - **Download it in Colab directly:**

     ```python
     !wget -q -O Tactile_DL_2027.zip https://github.com/LannWei/Deep-Learning-CourseWork-2027/releases/latest/download/Tactile_DL_2027.zip
     !unzip -q -o Tactile_DL_2027.zip -d /content
     ```

   - **Or download it to your computer** with
     [this link](https://github.com/LannWei/Deep-Learning-CourseWork-2027/releases/latest/download/Tactile_DL_2027.zip),
     then upload it to Google Drive or Colab. See Section 3 of the dataset README.

   Note: **Code → Download ZIP** does *not* include the dataset.
2. Read `/content/Tactile_DL_2027/README.md`.
3. Look at `example_submission/`. It is a complete, working submission with a small
   baseline CNN. Your own submission must use the same interface.

A GPU runtime in Google Colab (*Runtime → Change runtime type → GPU*) is enough for this
coursework.

---

## What to submit

> **Deadline:** `TBD` **Where:** `TBD`

### Part A

1. **Report (PDF).** IEEE double-column format, 3–6 pages, with these sections:
   Abstract, Introduction, Objectives, Methodology, Experiments, Evaluation, Conclusions
   and Future Work. Follow `2027_Deep_Learning_Report_Guidance.pdf`.
2. **Code.** Your scripts or notebooks for data preprocessing, model training, evaluation
   and tuning.
3. **Models.** A folder named after your student ID, containing:
   - `predict.py`, which runs inference for **both** tasks
   - your trained weights
   - any helper modules that `predict.py` imports
   - optionally, a `requirements.txt` listing extra pip packages

   `predict.py` must follow the interface in Section 4.3 of the dataset README. Run the
   self-check described there before you submit. **Submissions that do not follow the
   interface cannot be scored on the hidden test set.**

### Part B

4. **Video presentation.** Length: `TBD`. Format: `TBD` (e.g. MP4).

---

## Report template

Use the official IEEE conference template (LaTeX or Word):
<https://www.ieee.org/conferences/publishing/templates>

On Overleaf, search the template gallery for "IEEE Conference Template".

---

## Background reading

These papers give background on the dataset and on vision-based tactile sensors.

1. L. Wei, G. Khurana, S. Bhouri, W. Hong, Z. Xin, Q. Cong, W. Fan, Y. Xiang and D. Zhang,
   "TacVerse: A Multisensor Dataset and Benchmark for Cross-Sensor Vision-Based Tactile
   Perception," *Advanced Robotics Research*, 2026.
   [PDF](https://advanced.onlinelibrary.wiley.com/doi/pdf/10.1002/adrr.70169)
   · [doi:10.1002/adrr.70169](https://doi.org/10.1002/adrr.70169)  
   *The source of the coursework dataset.*
2. Q. Cong, S. Oh, W. Fan, S. Luo, K. Althoefer and D. Zhang, "TacEva: A Performance
   Evaluation Framework for Vision-Based Tactile Sensors," *Advanced Intelligent Systems*,
   2026. [PDF](https://advanced.onlinelibrary.wiley.com/doi/pdf/10.1002/aisy.202501179)
   · [doi:10.1002/aisy.202501179](https://doi.org/10.1002/aisy.202501179)

Dataset code: <https://github.com/LannWei/Tactile_Database>

---

## Questions

Please ask questions in `TBD` (e.g. the course discussion forum), so that everyone can see
the answers.
