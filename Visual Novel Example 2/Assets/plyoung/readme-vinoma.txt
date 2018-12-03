Vinoma
Copyright (c) 2015 Leslie Young

information and docs: 
https://plyoung.github.io/vinoma.html

videos:
https://www.youtube.com/playlist?list=PLuaBtUXEKcdJVi1eJIqIXqGcyNfU4la_5 

support:
http://forum.plyoung.com/c/vinoma/

-----------------------------------------------------------------------------------------------------------------------

Vinoma is a no-scripting/ programming solution for creating Visual Novel type games via a drag-and-drop interface.

- No programming/ scripting required
- Drag-and-drop actions to build scenes
- Easily change game's user interface (uGUI)
- Support for loading and saving
- Build-in localization support
- Distributed as DLLs for cleaner project
- Runtime source included for tinkerers (C#)

-----------------------------------------------------------------------------------------------------------------------

Other Kits
----------

** Blox Visual Scripting **

Vinoma includes an Action to trigger Blox Events. Import the package located under
`Assets/plyoung/vinoma/Packages/vinoma_blox.unitypackage`


-----------------------------------------------------------------------------------------------------------------------

This is quick guide on getting started. Please have a look at the video tutorials to learn about the various features of this system.

The Vinoma Editor can be opened from the Unity menu: `Window > Vinoma Editor`. It will cause two panels (windows) to open, the Vinoma Actions and Vinoma Main Editor/ Canvas.

Main Scene
----------

Vinoma has one main Unity Scene which controls the game. This scene is automatically created under `Assets\projectData\vinoma\MainScene` when you open the Vinoma Editor for the first time. Do not move or rename this scene. You might want to open it when you are ready to edit the GUI to your game's needs or want to add custom game scripts or other objects.

You will notice that there are 4 objects in this scene. Do not rename or delete them.

The first one is **VinomaGUI**, this is where all the user interface elements are defined in various panels. These include things like the main menu, buttons to load a session, and the settings panel. There are also important panels in here that works together with Actions during the game's run-time. The Dialogue action is one of the actions that needs a panel under the GUI to function correctly.

**VinomaGameGlobal** contains important objects and scripts for Vinoma to function. Do not editor anything on this object.

**_CustomScripts_** is where you will attack any custom script you create that contains functions you will invoke via the Scripts action.

You will add sprites and objects that you want to hide and show via the GameObject action under the **_GameObjects_** object.

Vinoma Scenes
-------------

A Vinoma based game consists of various Scenes that are build up from Actions. You drag and drop these actions into the Vinoma Canvas to build a scene. Actions are always executed from top-down but some actions can cause execution to branch off to another scene or to skip actions or even go back to previous actions.

When a new game is started Vinoma will start execution of actions from the very 1st action in the 1st scene of the list of Vinoma Scenes.

Vinoma is that easy to use. Have a look at the Actions page in the documentation to learn more about what each Action does and how to use them.
