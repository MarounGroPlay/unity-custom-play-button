# Unity Custom Play Button

This Fork is to add Addressables scenes . As Addressables does not exist in Editor build , Some chose to add then and turn the checkbox off ( That should work with original script) but i chose to not add them so i know which scenes are built in and which are addressables .
actually thats how the code detects if the scene should be loaded as addressable or not .

Original link https://github.com/antonysze/unity-custom-play-button

Add 2 custom play buttons to the Unity Toolbar to avoid keep switching scenes when testing the game. Directly play the game (the first scene in build setting) or specific scene (chose from dropdown list) by clicking those buttons without changing scene. When stop playing, scene will change back to the scene before play.  Additional dropdown list for quick build scene or bookmarked scene switching without searching it.

![image](https://user-images.githubusercontent.com/3353695/148316557-47d93af2-fb9d-46b8-97da-9ce409e02317.png)

## Installation
Import this from Unity Package Manager. You can [download and import it from your hard drive](https://docs.unity3d.com/Manual/upm-ui-local.html), or [link to it from github directly](https://docs.unity3d.com/Manual/upm-ui-giturl.html).

## Requirements
**Tested Unity version:** 2021 - 2019

Please make sure following package is installed to make this package works:
- [unity-toolbar-extender](https://github.com/marijnz/unity-toolbar-extender) - 1.4.1 or above

You can also install the prerequisite package via popup window after you installed this package:
![image](https://user-images.githubusercontent.com/3353695/148312273-2188311b-fe3e-4a4b-87ea-00ccaead8aef.png)

## How to use
![image](https://user-images.githubusercontent.com/3353695/148320339-2efc85a4-fc4b-44d7-bd84-662ff9e34c52.gif)

### Play Buttons on Unity Toobar
![image](https://user-images.githubusercontent.com/3353695/148315309-e6369f75-5a44-4684-8848-f59341058443.png)
1. **Dropdown button of custom scene** - open scene selection window
2. **Play custom scene button** - play target scene from dropdown button
3. **Play game button** - play the game (the first scene in build setting)

### Scene selection window
![image](https://user-images.githubusercontent.com/3353695/148323734-6bc75ebb-a3f7-4791-a865-5da002d43d49.png)

4. Select custom scene (for **play custom scene button**)
5. Bookmark/Unbookmark
6. Open scene in scene view
7. Select bookmark scriptable object
8. Unbookmark

### Scene Bookmark
Please note that bookmark is stored in a bookmark scripable object in your project. Please add to .gitignore if you do not want to share it. This scriptable object will be automatucally created from `Assets/Editor/CustomPlayButton/BookmarkSetting.asset`. You can also edit or reorder the list of bookmarks by modifying the scripable object directly.
