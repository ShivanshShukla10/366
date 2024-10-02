# 366

drive link https://drive.google.com/drive/folders/1iCdpPJfbbS58s9xTkoHlpi1CNEDYvlaG

[irds dataset](https://zenodo.org/record/4610859)
[irds eda github repo](https://github.com/alina-miron/intellirehabds)
--- 
## IRDS
Dataset Overview:
The dataset contains recordings of physical rehabilitation movements performed by 29 subjects (15 patients and 14 healthy controls). It includes 9 different gesture types, with multiple repetitions of each gesture.

File Structure and Naming Convention:
The dataset consists of 2589 files, each corresponding to one gesture performance. The file naming convention is as follows:

SubjectID_DateID_GestureLabel_RepetitionNo_CorrectLabel_Position.txt

For example: 303_18_4_10_1_stand.txt

- SubjectID: Unique identifier for each subject (e.g., 303)
- DateID: Identifier for the recording date (e.g., 18)
- GestureLabel: Number (0-8) corresponding to the gesture type
- RepetitionNo: The repetition number of the gesture (e.g., 10)
- CorrectLabel: 1 for correct, 2 for incorrect, 3 for poorly executed
- Position: The position in which the gesture was performed (e.g., stand, sit)

Data Dimensions and Content:
- Each file contains data for one gesture performance
- Data is recorded at 30 frames per second
- Each frame contains spatial information for 25 joints
- Each joint is represented by 3 coordinates (x, y, z)
- Total features per frame: 25 joints * 3 coordinates = 75 features

File Formats:
1. Simplified CSV format:
   - Each line contains the 3D coordinates of the 25 joints
   - 75 comma-separated values per line

2. Raw data format:
   - Includes timestamp for every frame
   - Information on whether each joint is tracked
   - 2D projections of the 3D coordinates

Additional Data:
- Raw depth map images are provided with the same naming convention as the corresponding .csv files

Data Statistics:
- Minimum gesture sequence length: 13 frames
- Maximum gesture sequence length: 1586 frames
- Average gesture length: 84 frames
- 75% of gestures have fewer than 89 frames
- Incorrect gestures tend to be longer (avg. 148 frames) than correct ones (avg. 68 frames)

Gesture Types:
0. Elbow Flexion Left
1. Elbow Flexion Right
2. Shoulder Flexion Left
3. Shoulder Flexion Right
4. Shoulder Abduction Left
5. Shoulder Abduction Right
6. Shoulder Forward Elevation
7. Side tap Left
8. Side tap Right

Subject Information:
- 15 patients (IDs 201-216)
- 7 physiotherapists (IDs 101-107)
- 7 physiotherapy students (IDs 301-307)

The dataset is designed to be used for assessing the performance of patients during simple rehabilitation movements and comparing them with a control group of healthy individuals.

---
