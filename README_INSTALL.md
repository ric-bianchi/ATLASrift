# ATLASrift
 ATLAS experiment at CERN - VR experience and Event Viewer

# Installation

1. Install Unreal Engine 4 from Epic Games (Free)
2. Install Visual Studio 2015 Community edition (Free)
3. Install Oculus Rift Runtime:
     https://developer.oculus.com/downloads/
4. Download the ATLASRift code repository from GitHub


# Running:

1. Double click on ATLASRift.uproject file. If Unreal Engine Editor does not start, link the .uproject extension to the Unreal Engine Editor binary.
2. Then click on the little arrow beside the Play button and choose `VR Preview`


# Technical details:

* before compilation unzip in-place Content/Detector/cavern/UX15elements.zip - this asset contains the cavern scafolding and is by default hidden. It can be shown by pressing "-" key, but expect performance to drop.

* There are two modes that can be set up with Rift and the one you want is "direct to rift".

* Also, there is setting in Windows on how the two displays are arranged so you may have to play a bit there. But that's done only once.

* When you run ATLASRift (by simply pressing "Play") you can switch to Oculus by pressing `<ALT>+<ENTER>`
* If you had ATLASRift Unreal project opened when you installed the Oculus Rift runtime, you will see the "VR Preview" option in Unreal greyed out. Please restart Unreal Engine.

# Update the ATLASRift project:

When you want to update your copy of the ATLASRift project with the latest changes from the developers:

- If you use **GitHub Desktop**:
  - Open GitHub Desktop
  - Click on the "Sync" button on the upper-right part of the window. This will pull all the changes from the remote repository. Pay attention, though: the "Sync" command will also push your local changes to the remote repository (but here we assume you are expert enough on GitHub if you made local changes to your local ATLASRift code base, so you will know how to handle that...)

- If you want to do it from the **command-line**:
	- Open the Windows "Command Prompt"
	- go to the folder where you extracted the ATLASRift code (for example: `C:\ATLASrift\`)
	- type the command: `git pull` (we assumed you have already installed `git` on your machine, together with the command-line commands). This will pull the changes from the remote repository to your local one.

If you update your project from a quite early version, you might be asked to install the *"Substance"* plugin from the Unreal Engine marketplace. It is a free plugin that allows us to use the "substance" files for advanced texturing. You can feel safe to install it.

You might also be asked for the permission to rebuild *"missing .dll modules"*; please answer yes and rebuild them.

If the Engine cannot build the necessary code, it will ask you to open the project in MS Visual Studio and build it manually.

Sometimes it cannot build it because you have to enter your MS credentials (the Microsoft account you have created/used when installing Visual Studio) again in MS Visual Studio, to make it working again.
Some other times, specially when updating a project to a newer version of Unreal Engine, a clean build of the whole project can help (right-click: `clean`, then right-click: `build`)
