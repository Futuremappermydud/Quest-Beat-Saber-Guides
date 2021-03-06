# Guide to Making Custom Bombs for BMBF

###  iplay games!#8247‘s (or Futuremappermydud) Guide to making custom bombs for the BMBF, and other quest mod loaders.

#### DISCLAIMER: Making custom bombs / getting custom bombs to work may require you to reset your assets (thus making you sort your songs again) multiple times, so losing all your song data is not uncommon, I am not responsible for you needing to reset your assets so don't complain about it to me or else

# Table of Contents

1. [Useful Links](#useful-links)
2. [Required Programs/Files](#required-programs-and-files-for-making-a-bomb)
3. [Get Your bomb Model](#get-your-bomb-model)
4. [Converting Your Objects to a Mod](#converting-your-objects-to-a-mod)
5. [Add Your bombs to the Repo](#add-your-bombs-to-the-repo)

# Other guides by me:
# Useful Links and stuff

- [BMBF by the Unicorns](https://github.com/emulamer/BeatOn/releases)
- [Sidequest Discord](https://discord.me/sidequestvr)
- [Beat Saber Modding Group Discord (BSMG)](https://discord.gg/beatsabermods)
- [Fusion360](https://www.autodesk.com/products/fusion-360/students-teachers-educators)
- [Blender(best choice)](https://www.blender.org/)
- [Custom Sabers](https://github.com/RedBrumbler/BeatOnCustomSabers/tree/master/Sabers)
- [Custom Blocks/Notes](https://github.com/RedBrumbler/BeatOnCustomSabers/tree/master/NoteCubes)
- [Other Asset Mods](https://github.com/RedBrumbler/BeatOnCustomSabers/tree/master/MiscAssetMods)

# Required Programs and Files for Making a bomb:

- Unity version [2018.3/4.10f1](https://unity3d.com/get-unity/download?thank-you=update&download_nid=61246&os=Win) or higher (any lower and BeatSaber will crash)
- Model program of your choice (I prefer blender, but RedBrumbler is wierd and likes Fusion360)
- UnityAssetBundleExtractor [(UABE)](https://mega.nz/#!eRY3gAAI!wEB5cTEAxtEEbe7jIKroatUxwYtwmcUnCjAzoMBEyCs)
  *NOT my program, be careful when downloading programs from the internet!*
- The [Guide Files.zip]() Contains an .blend with examples for modeling,obj of retro note example, and a beatonmod.json
# Get Your bomb Model
Making your own model:
------

You can also make your own model!

I will not make this guide on how to use model software to do so, just how to export the file from your model program to something usable for making the bombs.saber

For example, this bomb I made is based on a retro feel: This is also what it should look like when we are done

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.01%20retro%20preview.PNG)

once you have your model

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.1%20model%20preview.PNG)

you want to create a folder you will remember

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.2%20create%20memorable%20folder.PNG)

Next export the model to this folder as bomb.obj

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.3%20export%20to%20folder%20as%20bomb.obj'.PNG)

Converting Your objects into a mod
====== 
After getting your .obj file, you’ll be able to make them into a mod compatible with Beat Saber for Quest

You’ll start by installing unity version 2018.3/4.10f1 and create a new project(this may take a second)

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.4%20create%20unity%20project.PNG)

Open that unity project and delete camera and light so we can begin

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.5%20delete%20bad%20stuff.PNG)

Move in the .obj file

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.6%20insert%20obj.PNG)

So we can build the bomb, move them into the left field of unity

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.7%20move%20to%20left%20field.PNG)

Raw Unity Mesh Files
------
Now that your bomb is in unity, it’s time to convert them into raw unity mesh files. To start off with that, you’ll need to build the scene, press Ctrl + shift + b to open build settings, and build the scene for windows, mac and linux

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/0.8%20build%20scene.PNG)

Let it build in a folder of your choice (I would create a new folder called "Bomb_Build") and open UABE

![alt text](https://github.com/Futuremappermydud/Quest-Beat-Saber-Guides/blob/master/images/GuideFiles%20Bomb/1.0%20uabe%20screen.PNG)
Once in UABE, go to file -> open and navigate to the folder you built the scene in.

Inside the build folder should be a folder called <unityprojectname>_data, go into that folder and open sharedassets0.assets with UABE

![alt text](https://github.com/Futuremappermydud/Quest-Beat-Saber-Guides/blob/master/images/GuideFiles%20Bomb/0.9%20open%20shared%20assets%20with%20uabe.PNG)

You’ll get this screen, and your model will have a name, The name should be default
click the mesh and click export raw (!IMPORTANT! NAME THE .dat bomb.dat with no caps)

![alt text](https://github.com/RedBrumbler/BeatOnCustomSabers/blob/master/Guidefiles/modfiles5.png)

Put the .dat file in a folder that is the name of your bomb or whatever you want to call it.

![alt text](https://github.com/Futuremappermydud/quest-beat-saber-guides/blob/master/images/GuideFiles%20Bomb/1.1%20bomb.dat%20stuf.PNG)

Now to make the actual mod, if you haven’t already downloaded the Guide Files then use this link> (https://github.com/Futuremappermydud/Quest-Beat-Saber-Guides/blob/master/guidefiles/GuideFilesBomb.zip?raw=true) and open the beatonmod.json in a text editor vscode is my favorite.



### Taking a Picture of Your bomb


Before starting, you will need to zip your bomb up and drag it onto BeatOn's Upload screen. Make sure it is installed.

1. Start Beat Saber (not through BeatOn as this will cause the Quest's screencapture capabilities to not work)
2. Head to the tutorial
3. Go back to the Quest home screen and click "Sharing" at the bottom
4. Click record
5. show a clip of of the bomb in use
7. Plug your Quest up to your PC
8. Open SideQuest
9. Go to the "Files" tab
10. Head to the Oculus -> videoshots folder
11. Export to your bombs's folder
12. export the video to a location on your pc, open the video and find a good spot to take a screen shot (or convert to a gif). Save the screenshot/gif in your bomb's folder

At the top(or bottom) of the json you’ll see this info, now all you have to do is input your own info in there and name things correctly.
I recommend to only change the id, name, author, description and version numbers

```
"id": "ModID",
  "name": "Mod name",
  "author": "YourName",
  "description": ["Mod Description"],
  "gameVersion": "1.3.0p2",
  "version": "v1.0",
  "platform": "Quest",
  "category": "Other",
  "coverImageFilename": "Cover.png",
  "components":
```

for my sword I changed it to this:

```
"id": "retrobombv1", 
  "name": "Retro Bomb",
  "author": "Futuremappermydud", 
  "description": ["Retro Bomb innovation"], 
  "gameVersion": "1.3.0p2",
  "version": "v1.0", 
  "platform": "Quest",
  "category": "Other",
  "coverImageFilename": 
  "components":
```



Now that you have all your files ready you can bundle them into a zip file (winrar or 7zip work fine for this) make sure your zip file contains:
- beatonmod.json
- bomb.dat
- Cover.png(not needed to upload)

#### A .rar file won't work! It has to be .zip!

Now you should be ready to upload to BeatOn!

If you get "invalid mod", you likely are missing an argument in the info part I just listed, make sure all of it is there!

If it doesn’t work you might have to reset your assets (will lose all loaded songs, be careful!) but pressing reload songs will load back most of them, if it says invalid mod file you might miss some files or made an incomplete json

If bombs (even confirmed working ones) don't show up at all then you might even need to completely reinstall beat saber

# Add Your Bombs to the Repo(DO NOT ADD TO THIS REPO THIS IS NOT A MOD REPO)
(link to reds repo https://github.com/RedBrumbler/BeatOnCustomSabers)
RedBrumbler also supports adding your own bombs to the repository here!
(explanation adapted from @Yuuki#0802 from BSMG, and by that RedBrumbler means mostly blatantly copied)

1. Make a Github account if you haven't already
2. Click the "fork" button in the top right of reds repository
3. Download [github desktop](https://desktop.github.com/)
4. Go to your forked repo (so, yourname/BeatOnCustomSabers) and click "Clone or Download", Copy that link
5. Go to Github Desktop: File -> Clone repository -> URL and paste the link, then click clone (keep note of the local path you put the repo in)
6. Head to where you saved the repo in your file explorer (C:\User\GitHub\BeatOnCustomSabers)
7. Go to the "NoteBombs" folder.
8. Create a new folder for your bombs (ex. "LaBandit915's bombs")
9. Drag your zip file in this folder
10. Head back to Github desktop
11. Add a summary for your commit at the bottom left (ex. "Added {BombName} by LaBandit915")
12. Press commit
13. Press push
14. Go back to your forked repo and press "Create pull request" and submit!

***Once RedBrumbler or Yuuki accepts your pull request your bomb(s) will be added there!***

**Please test your mods before submitting to the repo. Make sure they have correct JSON formatting and appear correctly on the BeatOn mod screen.**
