<div align="left">
    <img src="code/aligned/app/static/images/logo.svg",style="height:50px;"> 
</div>

## Project Description
Aligned is a yoga pose correction web app that processes video of a user’s yoga pose and provides feedback on how to improve the pose. The app was built using Flask and runs on an Amazon EC2 instance with GPU for deep learning.

Aligned was selected by USF faculty as one of the top apps of 2019 and, as a result, our team had the opportunity to present the app to a panel of VCs. We plan to continue developing Aligned as a side project in the near future. *Please note that the app's website is not currently operational due to the high cost of continuously running the EC2.*

## How does it work?
**[Watch Demo Video](https://www.youtube.com/watch?v=t8HMLYR1-FE&feature=youtu.be)**

 - User logs in and selects which pose to evaluate
 - App provides instructions on how to execute the pose
 - Once ready, the user records a video of themselves doing the pose within the app (using webcam)
 - Video is automatically processed using [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose), an open-source, deep learning-based library for keypoint detection.
 - The app uses the keypoints from OpenPose to classify different pose faults using a rule-based system.
 - Feedback is provided to the user on how they can safely improve their pose.

## Important Links
 - [Final Presentation Slides to VCs](https://github.com/ecalkins/aligned_yoga_app/blob/master/Aligned_VC_Presentation_Deck.pdf)
 - [Flask routes](https://github.com/ecalkins/aligned_yoga_app/blob/master/code/aligned/app/routes.py)
 - [Video processing script](https://github.com/ecalkins/aligned_yoga_app/blob/master/code/aligned/process_openpose_user.py)
 - [Modeling](https://github.com/ecalkins/aligned_yoga_app/blob/master/code/aligned/modeling.py)
 - [OpenPose research paper](https://arxiv.org/pdf/1611.08050.pdf)
 
 ## Contributors
[Katja Wittfoth](https://github.com/katjawittfoth), [Brian Dorsey](https://github.com/bdorsey2), [Quinn Keck](https://github.com/keck343), [Evan Calkins](https://github.com/ecalkins), [Sankeerti Haniyur](https://github.com/skhaniyur), [Connor Swanson](https://github.com/conswanson), [Maria Vasilenko](https://github.com/mashamasha)
 
