The framework is implemented and tested on Unreal Engine v4.26.2. 
You can dowmload the framework and a sample generated dataset [here](https://cloud.dfki.de/owncloud/index.php/s/XfJ6L6yzFekZMSx)

For the automatic video recording option:

1. Download the SynthoGestures.zip
2. Install the open-source plugin [UEVideoRecorder](https://github.com/ash3D/UEVideoRecorder) with the required prerequisites and add to the Plugin Folder.
3. Open the project with Unreal Engine and install Unreal Engine suggested Plugins.
4. Once done, press “Play” to start the gesture implementation and recording.

For use without External Plugins, Download the SynthoGesture_without_External_Plugins.zip and skip step 2 from the above instructions, then use any screen capture and recording software to extract the gestures.

To create new cameras and gestures, you can either use the corresponding JSON files in the content folder or change them directly in the “actorSettings” option in the Unreal Engine scene.

The "Synthetic_Gestures_Dataset_Depth_Camera.zip" contains an example of the generated hand gestures for the six classes mentioned in the paper.
