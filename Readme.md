# SynthoGestures #
- This repository has the SynthoGestures Framework presented in the following papers: 
  - [Advancing Dynamic Hand Gesture Recognition in Driving Scenarios with Synthetic Data](https://doi.org/10.1145/3581961.3609889) at AutomotiveUI WIP 2023
  - [SynthoGestures: A Novel Framework for Synthetic Dynamic Hand Gesture Generation for Driving Scenarios](https://doi.org/10.1145/3586182.3616635) at UIST Poster 2023

![alt text](https://github.com/amrgomaaelhady/SynthoGestures/blob/main/Fig.png)

- - -

The framework is implemented and tested on Unreal Engine v4.26.2. 
You can dowmload the framework and a sample generated dataset [here](https://cloud.dfki.de/owncloud/index.php/s/XfJ6L6yzFekZMSx).

For the automatic video recording option:

1. Download the SynthoGestures.zip
2. Install the open-source plugin [UEVideoRecorder](https://github.com/ash3D/UEVideoRecorder) with the required prerequisites and add to the Plugin Folder.
3. Open the project with Unreal Engine and install Unreal Engine suggested Plugins.
4. Once done, press “Play” to start the gesture implementation and recording.

For use without External Plugins, Download the SynthoGesture_without_External_Plugins.zip and skip step 2 from the above instructions, then use any screen capture and recording software to extract the gestures.

To create new cameras and gestures, you can either use the corresponding JSON files in the content folder or change them directly in the “actorSettings” option in the Unreal Engine scene. Check the below image for where can you activate different cameras, and select one of the implemented gestures. You can change all what you need from "SettingsActor" block (sorry the name was reversed in the readme and I have changed it now). You can either find it in the "World Outliner" window or there is a rectangular block in the scene called "Settings" that you simply need to click. In the "Details" window of that block, you will have to expand everything in the Default section to see all implemented gestures and camera types. You could also simple duplicate the components in the Gesture List to make it do the gestures in sequence instead of playing them one by one.

![alt text](https://github.com/amrgomaaelhady/SynthoGestures/blob/main/Fig2.jpg)

The "Synthetic_Gestures_Dataset_Depth_Camera.zip" contains an example of the generated hand gestures for the six classes mentioned in the papers.

As for creating your own gesture, this would require familiarity with Unreal Engine a bit. Basically there a class Blueprint named "BasicSplineGesture" where all the implemented Gestures inherit from it. So, you would need to create your own class Blueprint that would inherit from the Basic one, but with different variations in the hand path, also named spline (for example, check "RotateGesture" Blueprint).

## Citation ##

- If you find this code helpful, please cite our papers:
```

@inproceedings{10.1145/3586182.3616635,
author = {Gomaa, Amr and Zitt, Robin and Reyes, Guillermo and Kr{\"u}ger, Antonio},
title = {SynthoGestures: A Novel Framework for Synthetic Dynamic Hand Gesture Generation for Driving Scenarios](https://doi.org/10.1145/3586182.3616635},
year = {2023},
isbn = {9781450384810},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3586182.3616635},
doi = {10.1145/3586182.3616635},
booktitle = {Adjunct Proceedings of the 36th Annual ACM Symposium on User Interface Software and Technology},
location = {San Francisco, CA, USA},
series = {UIST '23 Adjunct}
}

@inproceedings{10.1145/3581961.3609889,
author = {Gomaa, Amr and Zitt, Robin and Reyes, Guillermo},
title = {Advancing Dynamic Hand Gesture Recognition in Driving Scenarios with Synthetic Data},
year = {2023},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3581961.3609889},
doi = {10.1145/3581961.3609889},
booktitle = {Adjunct Proceedings of the 15th International Conference on Automotive User Interfaces and Interactive Vehicular Applications},
location = {Ingolstadt, Germany},
series = {AutomotiveUI '23 Adjunct}
}
```
- - -
