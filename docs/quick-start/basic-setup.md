## Import PrydeVR and Load the Example Scene

Make sure you have [SteamVR](https://www.assetstore.unity3d.com/en/#!/content/32647) plugin in your project (Required only for the example scene)

Import the PrydeVR Unity Plugin (currently distributed as a separate UnityPackage)

Under _Assets/PrydeVR/Scenes/_, open the example scene

Hit play to start the demo

!!! note
    You should be able to see a big panel in front of you called _PrydeVR Live View Panel_. The panel will stream PrydeVR's camera view so you can clearly see what's going on

    We've configured PrydeVR camera using the _Orbit Smooth_ mode. You should be able to see a small camera preview panel floating in the air that is orbiting around you. If you find it, say hi to our VR camera rig! We embedded the preview panel so it's easy for players to find the camera and be able to see what the camera sees. You can easily turn it off in the PrydeVR control panel if you don't need it.

    By default, the recording can be started and stopped by pressing the X key in your keyboard. We provided other mapping options including some that use the Vive Controllers. You can change them in the PrydeVR gameobject. We also have an easy to use voice command system setup if you would like to use your own voice to control the recording.


**Press X key to start record**. Alternatively, you can use our built-in voice command system (requires Internet connection). Simply say out loud _"start recording"_ to start. Once you started recording, you should see the camera preview panel start to blink red indicating the capturing has already started.

!!! note
    Feel free to move around and teleport. The PrydeVR camera will smoothly follows you as you move.

**Press X again to stop recording**. If you prefer using voice command, just say out loud _"stop recording"_ to stop. By default, video file will be created in the "PrydeVR" folder under current Windows user's Documents folder. However, you can easily customize the output folder in the PrydeVR control panel. The path to the file will also output to the console window.

!!! note
    You can record as many times as you want and each session will create a separate video file.

   <center>
     <img src="../../Imgs/v0.3_FilePath1.png" alt="Saved file path">
   </center>

---

## Apply PrydeVR to Your Own Game

1. Open SteamVR interaction system example scene located at: Assets/SteamVR/InteractionSystem/Samples/Scenes/Interactions_Example
2. Drag the PrydeVR prefab under _Assets/PrydeVR/Prefabs/_ to anywhere in your scene hierarchy
3. All done. No kidding! Now hit play and you should be able to record and share!

!!! note
    Pretty easy-to-use, right? Now that you are all set with the setup, keep in mind that we also support you with many options to fully customize PrydeVR the way you like.

Select the PrydeVR gameobject that you just imported in your scene hierarchy and you should see the PrydeVR control panel. Let's go through every single one of them in the next section.

<center>
    <img src="../../Imgs/InspectorUI.png" alt="Saved file path" width="300" align="center">
</center>

---

## Customize Your Own Camera Rig
PrydeVR now supports customizing your own camera rig since SDK v0.5.0. This allows you to fully customimze the recording camera the way you want. Below is an example taking use of the custom camera feature to make a hand-held camera rig in under 60 seconds.

First, make sure PrydeVR SDK is already imported to you Unity project.

Under _Assets/PrydeVR/Scenes/_, open the example scene

Click PrydeVR gameobject again, find *Camera Follow Regime* and select *Custom Camera*. Then leave *Camera Local Position* to (0, 0, 0) and update *Camera Local Rotation* to (**30**, 0, 0).

Enable *Show Camera Preview* and then update *Camera Preview Position* to (0, 0, **0.4**) and *Camera Preview Rotation* to (**60**, **180**, 0). Leave *Camera Preview Scale* to its default 1.

Now drag the *Hand1* gameobject under _Player/SteamVRObjects/_ to *Target Camera* to make the reference. Now you are all set! Your setting should looks like the example below.
  <center>
    <img src="../../Imgs/CustomCamera_InspectorField.png" alt="Saved file path" width="400" align="center">
  </center>

Go ahead hit play. Now you should be able to see a camera preview panel is attached to one of your "*hand*" and it has already becomes a camera rig.
