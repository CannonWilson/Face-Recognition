# Face Attendance

Kincannon Wilson Final Project for CS 771

---

### Description

This repo shows the final version of the project 
"Distributed Web-Based Facial Recognition for Student 
Attendance." This project is based on the project 
completed for the annual UW-Madison hackathon 
CheeseHacks, which my team won. My team contributed 
a great deal of work to the app so please look at their
info in the final presentation slides and check them out!

My paper's abstract does a fair job of summarizing the
project:

This project involves the creation of a web-based application 
capable of recognizing the faces of students as they walk in 
front of a camera in order to record their attendance. Images 
from a video stream on an instructor’s device are sent over 
HTTP to a server that 1. performs face detection using an MTCNN, 
2. detects spoofs with a liveness detection network based on ResNet-18
and trained on the [CelebA-Spoof dataset](https://github.com/ZhangYuanhan-AI/CelebA-Spoof), 
and 3. if a live face has been detected, generates an embedding of 
the image using Inception ResNet V1. The embedding is compared to 
known embeddings using cosine similarity to identify the student 
in the photo. 

For more info, please read the rest of the paper or 
look at the presentation. Also feel free to check out the code in the CheeseHacks repo 
since the code I submitted for CS771 made minimal functional changes over that repo.