---
label: Better Textures
icon: ":scream:"
order: 98
authors:
  - name: Break
    avatar: "https://cdn.discordapp.com/avatars/839279738882883624/196ce6eac04b46f137da549f0c16b6a4"
---
This comprehensive guide is tailored for players of Arma 2 DayZ Epoch who seek to enhance their gaming experience through improved textures. It focuses on leveraging the assets available in the Arma 2: Army of the Czech Republic DLC to bring a new level of visual fidelity to the game.   
The guide begins by outlining the basic steps for integrating the DLC into DayZ Epoch, ensuring compatibility and stability. It then delves into advanced techniques for texture enhancement, including detailed instructions on texture optimization tips for better performance. This guide is an invaluable resource for both novice and experienced players looking to elevate their Arma 2 DayZ Epoch experience.

## Steps
1. Go to your `Arma 2 Operation Arrowhead` folder which is located here:   
    `C:\Program Files (x86)\Steam\steamapps\common\Arma 2 Operation Arrowhead`
2. Find the `ACR` folder and make a copy of it, and rename the copy to `@ACR`
3. Move your `@DayZ_Epoch` folder into the `Arma 2 Operation Arrowhead` folder, the `@DayZ_Epoch` folder is typically located in   
    `C:\Users\[user]\Documents\mods`.
4. You'll either need to do one of two things:
   1. Download a pre-made .bat file and drag it into the `Arma 2 Operation Arrowhead` folder.
      [!file DayZ_Epoch.bat straight to the M.S.G server](/static/DayZ_Epoch.bat)
   2. Make a copy of the `_runA2CO.cmd`/`_runA2CO.bat` and rename it to whatever you want.
      1. Open up the copy you made of the `.cmd`/`.bat` file and find where it says this:
          ```
          "%_STEAMPATH%\steam.exe" -applaunch 33930 "-mod=%_ARMA2PATH%;EXPANSION;ca"
          ```
          and replace it with this:
          ```
          "%_STEAMPATH%\steam.exe" -applaunch 33930 "-mod=%_ARMA2PATH%;EXPANSION;ca;@ACR;@DayZ;@DayZ_Epoch" -nosplash -skipIntro -noPause
          ```
      2. (Optional) If you want it to go straight to the M.S.G server, you can add `-connect="213.166.86.65" -port="2302"` to the end of that.
5. Double-click the file, and you'll be good to go.