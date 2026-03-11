# prototype-jump-rope-competitive-style-detection
This repository trries to present a pose-estimaton based algorithm that returns the amount of rope skipping jumps in a video of a competitive skippier who follows competitive jump rope style.

Within the code one changes the inmput video and the fps of the video.
The code was developed in jupyter notebook, a web-based interactive computing platform
Important to note is that the code runs using pose_iter_440000.caffemodel which can be found here: https://huggingface.co/camenduru/openpose/tree/f4a22b0e6fa2a4a2b1e2d50bd589e8bb11ebea7c and pose_deploy_linevec.prototxt which can be found here: https://github.com/CMU-Perceptual-Computing-Lab/openpose/tree/master/models/pose/coco

There is no detection of a start or end of the movement, threrfore the video should be edited so that the video only includes the action itself.


This is a prototype and is in many sections not jet up to the task. 
Some issues lie in the pose estimation model itself which compromises resolution to achieve better runtime and confidence values which results in generally very general, non specific outputs. This can lead to some jumps being missed. It should only be used as a general value that depicts the area in which the final score lies.
