# ros2_ws_misr

ROS 2 workspace template for Docker with VSCode

### This is version for **Windows OS**. 

If you use Windows, switch to [**Ubuntu branch**](https://github.com/LRMPUT/ros2_ws_misr/tree/jazzy).


## Initial setup

1. &nbsp; Download [XLaunch Server](https://sourceforge.net/projects/vcxsrv/) and install.
2. &nbsp; Download [Docker Desktop](https://docs.docker.com/desktop/install/windows-install/) and install.
3. &nbsp; Download [Visual Studio Code](https://code.visualstudio.com/download) and install.
4. &nbsp; Open VS Code and install an extension (shortcut CTRL+SHIFT+X) with the name `"Remote Development"`.
5. &nbsp; Download [repository](https://github.com/LRMPUT/ros2_ws_misr/archive/refs/heads/jazzy-Windows.zip), unzip it.

## Clone the repository and open it in VS Code

1. &nbsp; Run XLaunch Server with default settings.
2. &nbsp; Run Docker Desktop (in the background).
3. &nbsp; Run VS Code and open a directory `ros2_ws_misr`
4. &nbsp; In VS Code
    - press button in the notification (bottom-right corner of the screen) `"Reopen in Container"`
    - OR press `F1` and type "Reopen in...", select `"Dev Containers: Rebuild and Reopen in Container"`, click Enter
    - Wait for the container to set up

## Setup ROS packages for class

Execute the setup script with the command:
```bash
./src/setup_ws.sh
```

Build the workspace:
```bash
colcon build --symlink-install
```

Source environment:
```bash
source install/setup.bash
```
