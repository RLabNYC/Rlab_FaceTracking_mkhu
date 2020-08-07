![Image of rlab](https://i.ibb.co/3zsstG6/Group-3.png)


# Authors

Todd Bryant, Kat Sullivan, Grant Ng and Jiuxin Zhu

# From the RLab!

To learn more about us visit our website [here](https://www.rlab.nyc/)


## MakeHuman example

Welcome to our **Makehuman** workflow! This is an example of what a makehuman model will look like with facetracking.

![gif of me](Media/rlabmkhu.gif)


### Required Software To Be Installed: 
* Blender here: https://www.blender.org/
* MakeHuman downloaded here: http://www.makehumancommunity.org/
* Maya student version download here: https://www.autodesk.com/education/free-software/maya
* Unreal downloaded here: https://www.unrealengine.com/en-US/get-now/agnostic
### Software versions:
* Unreal version 4.25 
* Live Link Face app for iOS (Requires iOS 13.0 or later). Compatable with iPhone, iPad, and iPod touch. 
* Maya 2018 or 2019
* Blender 2.83 

This tutorial requires some knowledge of using 3D software and game engine mechanics. We will provide more links for beginners that walk you through a more in depth overview. 


# Importing and Exporting free 3D characters blendshapes with Maya

### For experienced individuals only!
 - If you are an already experienced in facial tracking, you can download this repo and it will be ready to work with the livelink app already!

## For Beginners
 - This repo is mainly for beginners who want to get into facetracking for personal projects, virtual production or just for fun. Please keep in mind that this repo is for the Unreal engine.

 - First, you need to have the LiveLink app downloaded onto your iPhone before you start this tutorial. Then download or clone this repository somewhere on your computer. There are multiple ways to have a fully rigged character and have a facial rig set up in minutes. 

**1. Exporting blendshapes from Makehuman and importing into Blender into Maya**
  - **Getting the Blendshapes out of MakeHuman/Blender:**
     - The MakeHuman and Blender workflow integrates these two open source software platforms to extract the blendshapes associated with all of the parametric sliders for crafting your avatar.  You’ll need to install two plugins to MakeHuman and one to Blender. Both are free downloads and have robust communities.
  - **Editing Blendshapes in Maya from MakeHuman:**
     - Once you make the switch, you will see a bunch of orange targets, these are the blendshapes. You can toggle between how strong you want each target to be for animation purposes. It’s basically like a light dimmer. 
    -[Makehuman](http://www.makehumancommunity.org/content/downloads.html) (new link for community [edition](http://download.tuxfamily.org/makehuman/nightly/makehuman-community-1.2.0-alpha4-win32.zip))
    -[Blender](https://www.blender.org/download/)

![make human screen shot](https://i.ibb.co/8zsWQsh/Make-Human-Community-1-2-0-Beta1-HEAD-748a570b-Untitled-6-25-2020-5-08-27-PM.png)

**Installing the Plugins**
Once both are installed let’s grab the plugins and turn them on.

All the plugins needed are [on one page](http://www.makehumancommunity.org/content/plugins.html)

Under the Plugins for MakeHuman section download MHAPI and Forked MHX2. The Forked MHX2 has both the plugin for MakeHuman and Blender.

   - In MakeHuman:
        - [From the MakeHuman Documentation](http://www.makehumancommunity.org/wiki/FAQ:I_downloaded_a_third_party_plug-in._How_do_I_install_it%3F).
        - On PC the Plugins go in the “plugins” folder wherever you installed MakeHuman.

![mkhu pc set up](https://i.ibb.co/bH5HNKH/Work-flow-for-facial-tracking-Google-Docs-Google-Chrome-6-25-2020-6-36-48-PM-2.png)

   - On Mac the Plugins go inside the MakeHuman.app. Navigate to your Applications folder and right-click on your MakeHuman.app and select “Show Package Contents” and then put the plugins in this location. Note that it goes into the plugin folder in Resources, not the Plugin folder in the root Content folder.

![mac set up](https://i.ibb.co/DMpjfbW/Work-flow-for-facial-tracking-Google-Docs-Google-Chrome-6-25-2020-6-37-28-PM-2.png)

   - Copy the 9_export_mhx2 folder and paste it in the plugins folder where MakeHuman is installed.
   - Unzip MHAPI and copy the folder 1_mhapi in the same plugins folder where MakeHuman is installed. 

 - **In Blender:** 
    - Zip up the folder import_runtime_mhx2 and open the Blender application. Go to Edit -> Preferences -> Add-ons. Select “Install” and look for the zipped folder.
![blender set up](https://i.ibb.co/khfv10x/Work-flow-for-facial-tracking-Google-Docs-Google-Chrome-6-25-2020-6-59-29-PM-2.png)

    - Exporting from MakeHuman.
    - Create your avatar in MakeHuman. Put your character into a T-Pose before exporting.  Go to Files -> Export and Select MakeHuman Exchange (mhx2), then check the box for Poses on the right Options menu.  Blendshapes are called Targets in MakeHuman and they are used in the Poses.  If you do not see these options, check your plugin installation.

![Make human export](https://i.ibb.co/vQXVNdX/Work-flow-for-facial-tracking-Google-Docs-Google-Chrome-6-25-2020-7-36-36-PM-2.png)

  - **Importing into Blender**
  - Now Open Blender and navigate to File -> Import -> MakeHuman (.mhx2).  On the import window select your file from MakeHuman and Check the box on the right for Override Exported Data.  Under Import Human Type check Face Shapes. Under Rigging choose the Rig Type Humanik.

![Blnder set up](https://i.ibb.co/W54b0YG/blendersetup.png)

![Blender import](https://i.ibb.co/4gvR1gm/Blender-6-23-2020-8-21-51-PM-2.png)

  - Export as FBX from Blender. Turn off “Apply Modifiers” in the Geometry section of the FBX export options.
 

 # The next steps are [here](https://github.com/RLabNYC/Rlab_FaceTracking_mkhu/blob/master/RUNSCRIPT.md)

## If you need to go back to the table of [contents](https://github.com/RLabNYC/RLab_Facetracking). 

