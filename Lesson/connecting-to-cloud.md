# Connecting to the cloud computer instances
Having moved to a new computer classroom, we'll now need to slightly alter how we connect to the cloud computers.

## Linux (Ubuntu 14.04)
1. If this is the first time connecting, open a Terminal window (click Ubuntu icon on top left, enter "Terminal" in search box) and type

    ```bash
    $ vinagre
    ```
This will open the default Ubuntu Remote Desktop Viewer (**Vinagre**).
You can right-click on the icon and select **Lock to Launcher** to keep the icon there for future classes.
2. After **Vinagre** opens, you can click on the **Connect** button on the top left to make a new connection.
  - Select **VNC** for the Protocol
  - Enter the IP of the remote computer, plus the port number as the host: `XXX.XXX.XXX.XXX:5901`
  - I suggest you tick the boxes for **Fullscreen** and **Scaling**, which will make the window fill the screen. You should also leave the box for **Keep aspect ratio** ticked.
  - At this point you can click the **Connect** button.

**Note**: To exit full screen mode, press the **F11** key.

## Windows 7
### Remote Desktop Connection
1. Click on Windows start button.
2. Enter "Remote Desktop Connection" in search window.
3. [Connect as usual](https://github.com/Python-for-geo-people/Lesson-1-Course-Environment/blob/master/Background/connect-win-rdp.md).

### TightVNC
The TightVNC client should be available in Windows on these computers, so you should be able to [connect the same way we have previously](https://github.com/Python-for-geo-people/Lesson-1-Course-Environment/blob/master/Background/connect-win-vnc.md).
