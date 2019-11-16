# Documentations about various method of non-real-time recordings in Windows Games and Emulators

## Windows Games

TODO

## Emulators

### RPCS3 (PS3)

<details>
<summary>Windows</summary>

On Windows it's extremely easy to record videos. but in-game performance and stability will be lower compared to Linux.

Software:

  * Any recording software ([OBS](https://github.com/obsproject/obs-studio) as an example)
  * [Cheat Engine](https://github.com/cheat-engine/cheat-engine) (used to slow down the emulator)

1. Find your minimum and maximum framerate

I'll be using Killzone 2 Demo for this example.

Min FPS:

![](https://i.imgur.com/XwrnZds.png)

Max FPS:

![](https://i.imgur.com/7YJP2dL.png)

2. Preparing the recording

Go into CE settings and Hotkeys

Set your speed by dividing your minimum frame rate with your target video framerate (60 FPS in this example):

in my case 3 FPS is minimum. (3/60 = 0.05)

![](https://i.imgur.com/n11f69c.png)

Configuring RPCS3:

I'll be using the vblank method to unlock the framerate for this game.

You can use [Game Patches](https://github.com/RPCS3/rpcs3/wiki/Game-Patches) (if available for your game)

![](https://i.imgur.com/WYGrQVG.png)

Audio:

  * Untick Audio Buffering (VERY IMPORTANT)
  * Dump to file

![](https://i.imgur.com/Bwq2yNx.png)

3. Configure your recording software

Setup OBS to record at 30 FPS or higher. (This insure that there will be no skipped frames during the recording)
![](https://i.imgur.com/M6W76Nu.png)

Add the Game Window to your scene.

Once you're ready to record press your Hotkey button and start recording.

![](https://i.imgur.com/HPCDO18.png)

If you're recording multiple segments rename the audio file inside your RPCS3 folder from `audio` to anything else before starting another session of the game or else you'll lose your audio file.

4. Editing

You can use any editing software to post-process the recordings.

I'll be using [Adobe Premiere Pro](https://www.adobe.com/sea/products/premiere.html)

Set your project framerate to match the target video framerate (60FPS)

![](https://i.imgur.com/RvQFXVk.png)

Speed your video back up to 100% of realtime (2000% for 0.05)

Sync your audio you can use the waveforms for this.

![](https://i.imgur.com/jGXEUa7.png)

- Resulting [video](https://youtu.be/ST5VoVKJHno)

</details>


#### Linux

TODO


## Xenia (Xbox 360)
TODO


## PCSX2 (PS2)
TODO
