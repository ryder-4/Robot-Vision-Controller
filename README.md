# Robot Vision Controller
Hi! This Readme contains links to inference results, output videos, model weights, e.t.c. I hope they help in understanding the project.:)





### Task: 
Implement a vision based controller for a driving robot using the camera feed.

### Methodology:
1. Create a dataset from the camera feed
   * [Original Camera Feed](https://drive.google.com/file/d/1N9OdasASDit6Z_NXC7Jb_GalDBiU9RNh/view?usp=drive_link)
   * Total frames extracted from the video: 71
   * Train test split: 63 | 8
3. Annotate and augment it in Roboflow
   * No. of augmentations: 2
   * Augmentation types: Color grading, 180 rotation along the height axis
  
   
   | Original Frame | Augmented Frame 1 (Rotated and Color Graded)  | Augmented Frame 2 (Rotated and Color Graded) |
   | :---: | :---: | :---: |
   | <img src="https://github.com/user-attachments/assets/493c786b-f094-470a-b2bd-c05475deb0e3" width="200" height="200" /> | <img src="https://github.com/user-attachments/assets/ce44af7b-531a-4615-9ea2-ea4d1befbf15" width="200" height="200" /> | <img src="https://github.com/user-attachments/assets/578d386e-15be-4040-91ad-c9c794b89dc6" width="200" height="200" /> |

   * Total frames after augmentation: 213
   * Train test split: 187 | 26
   * Total frames after augmentation: 213
   * Train test split: 187 |  26 
   
5. Finetune a segmention model using the dataset
   * Model used: PIDNet
   * [Finetuned weights](https://drive.google.com/file/d/1htyHFWql19tBlLKyvZYXPsygilm_Gdpq/view?usp=drive_link)
  
7. Run inference on the model to generate a segmented output video
   * [Baseline inference](https://drive.google.com/file/d/13Ook0B9Y6k9UWbo7eipHhYE2T6AdQWUP/view?usp=drive_link)
   * [Finetuned inference](https://drive.google.com/file/d/10rI9E2w1nsRB8g0ScAo5qHlvR3sgNNQ4/view?usp=drive_link)
     
9. Implement a vision controller on the output video
    * [Vision Controller Output](https://drive.google.com/file/d/1gDD_qyZhDd_VrrWz3SYk2ky6JKP_VFhW/view?usp=drive_link)






