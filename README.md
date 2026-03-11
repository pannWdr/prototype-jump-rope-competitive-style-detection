# prototype-jump-rope-competitive-style-detection
This repository trries to present a pose-estimaton based algorithm that returns the amount of rope skipping jumps in a video of a competitive skippier who follows competitive jump rope style.

Within the code one changes the inmput video and the fps of the video.
Important to note is that the code runs using pose_iter_440000.caffemodel which can be found here: https://huggingface.co/camenduru/openpose/tree/f4a22b0e6fa2a4a2b1e2d50bd589e8bb11ebea7c

There is no detection of a start or end of the movement, threrfore the video should be edited so that the video only includes the action itself.


This is a prototype and is in many sections not jet up to the task. 
Major isses lie in the pose estimation model which compromises resolution which results in generally bad outputs.
