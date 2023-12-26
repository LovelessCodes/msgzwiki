---
label: Better Textures
icon: ":scream:"
order: 98
authors:
  - name: Break
    avatar: "https://cdn.discordapp.com/avatars/839279738882883624/196ce6eac04b46f137da549f0c16b6a4"
---
!!!
You will need to own [Arma 2: Army of the Czech Republic DLC](https://store.steampowered.com/app/33934/Arma_2_Army_of_the_Czech_Republic/) on Steam in order for this to work
!!!

This comprehensive guide is tailored for players of Arma 2 DayZ Epoch who seek to enhance their gaming experience through improved textures. It focuses on leveraging the assets available in the [Arma 2: Army of the Czech Republic DLC](https://store.steampowered.com/app/33934/Arma_2_Army_of_the_Czech_Republic/) to bring a new level of visual fidelity to the game.   
The guide begins by outlining the basic steps for integrating the DLC into DayZ Epoch, ensuring compatibility and stability. It then delves into advanced techniques for texture enhancement, including detailed instructions on texture optimization tips for better performance. This guide is an invaluable resource for both novice and experienced players looking to elevate their Arma 2 DayZ Epoch experience.

## Steps
1. Install `Arma 2: Army of the Czech Republic` by starting `Arma 2: Operation Arrowhead` on steam, and it'll ask you what you want to do, and there should be an option to install it
2. Go to your `Arma 2 Operation Arrowhead` folder which is located here:   
    `C:\Program Files (x86)\Steam\steamapps\common\Arma 2 Operation Arrowhead`
3. Find the `ACR` folder and make a copy of it, and rename the copy to `@ACR`
4. Move your `@DayZ_Epoch` folder into the `Arma 2 Operation Arrowhead` folder, the `@DayZ_Epoch` folder is typically located in   
    `C:\Users\[user]\Documents\mods`.
5. You'll either need to do one of two things:
   1. Download a pre-made .bat file and drag it into the `Arma 2 Operation Arrowhead` folder.
      [!file DayZ_Epoch.bat straight to the M.S.G server](/static/DayZ_Epoch.bat)
   2. Make a copy of the `_runA2CO.cmd`/`_runA2CO.bat` and rename it to whatever you want.
      1. Open up the copy you made of the `.cmd`/`.bat` file and find where it says this:
          ```
          "%_STEAMPATH%\steam.exe" -applaunch 33930 "-mod=%_ARMA2PATH%;EXPANSION;ca"
          ```
          and replace it with this:
          ```
          "%_STEAMPATH%\steam.exe" -applaunch 33930 "-mod=%_ARMA2PATH%;EXPANSION;ca;@ACR;@BAF;@PMC;@DayZ_Epoch" -nosplash -skipIntro -noPause
          ```
      2. (Optional) If you want it to go straight to the M.S.G server, you can add `-connect="213.166.86.65" -port="2302"` to the end of that.
6. Double-click the file, and you'll be good to go.

## Extra

We can do the same for [Arma 2: British Armed Forces](https://store.steampowered.com/app/65700/Arma_2_British_Armed_Forces/) and/or [Arma 2: Private Military Company](https://store.steampowered.com/app/65720/Arma_2_Private_Military_Company/)

Although the steps is a little different on this one, since they come as actual installables on Steam.

### Steps (Extra)
+++ British Armed Forces

1. Install the DLC on Steam of `Arma 2: British Armed Forces`
2. Start the DLC as you would a normal game, and it'll start installing the DLC
3. Go to your `Arma 2 Operation Arrowhead` folder which is located here:   
    `C:\Program Files (x86)\Steam\steamapps\common\Arma 2 Operation Arrowhead`
4. Rename the folder `BAF` to `@BAF`

+++ Private Military Company

1. Install the DLC on Steam of `Arma 2: Private Military Company`
2. Start the DLC as you would a normal game, and it'll start installing the DLC
3. Go to your `Arma 2 Operation Arrowhead` folder which is located here:   
    `C:\Program Files (x86)\Steam\steamapps\common\Arma 2 Operation Arrowhead`
4. Rename the folder `PMC` to `@PMC`

+++

If you followed the steps on `Army of the Czech Republic`, you should be good to go, since we already prepared the `.bat`/`.cmd` file to run all the DLCs you've installed.

Otherwise just add either `@PMC;` or `@BAF;` after `@ACR;` in the `.bat`/`.cmd` file.

## Troubleshooting

=== *I'm getting "MISSING STRING" when trying to install `Army of the Czech Republic`*

This will happen if you've not opened `Arma 2` or `Arma 2: Operation Arrowhead`.
In-order for it to work, you should've at least opened both once.

==- *I can't find the `ACR` folder in my `Arma 2 Operation Arrowhead` folder*

Be sure to have installed `Army of the Czech Republic` before-hand.

Check step 1.

==-