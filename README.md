# Face Recognition

During my first semester of my master's program in Fall '22, I got interested in applications of machine learning. The course I TA'd for took attendance using notecards with each student's name written on the notecard. I thought it would be a good project to implement a facial recognition-based attendance system for use in courses like mine. 

The first step (Flask-Uploads) was a basic app with a React frontend and Flask backend.

Next, I was lucky enough to join UW-Madison's biggest annual hackathon (CheesHacks) with a team of 3 other students. We built a functioning facial-recognition attendance system with a polished UI. We won the competition and the $500 grand prize!

Finally, I used my experience during CheeseHacks to write a paper and give a presentation for my CS771 course (on deep learning methods for computer vision) on the feasibility of a one-shot system for facial recognition.

Each directory in this repo contains the project code, along with explanations and screenshots.

## CheeseHacks

This submission won the UW-Madison CheesHacks hackathon in Fall '22! We started by recreating my base project (Face-Attendance). Then, we created a more polished frontend and implemented a face recognition system on the backend that works by calculating the cosine similarity between image embeddings.

Technologies used:

- Flask backend
- React frontend
- Multi-Task Cascaded Neural Networks (MTCNN) for fast face detection
- Inception Resnet V1 for generating image embeddings

## CV771-Report

The final version of the facial-recognition-based attendance system builds on top of the CheeseHacks project with a liveness detection check. This repo also contains a report I wrote and a presentation I gave for my CS771 class.

Technologies used:

- Same as CheeseHacks project above
- Resnet-18 network trained on CelebA-Spoof dataset for liveness detection
- LaTeX

## Flask-Uploads

This app served as the basis for the other two above. The app has a React frontend that lets users create classes and upload images of studens. The Flask backend stores uploaded images on the server computer. 

Technologies used:

- Flask backend
- React frontend