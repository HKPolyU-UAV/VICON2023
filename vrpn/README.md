# VRPN Settings

1. **Install**
    ```
    sudo apt update
    sudo apt-get install ros-noetic-vrpn ros-noetic-vrpn-client-ros
    ```
2. **Remap**
   
   In ```vrpn.launch```, modify the object name:
   ```
   <remap from="/vrpn_client_node/{your_object_name}/pose" to="/mavros/vision_pose/pose" />
   ```
3. **roslaunch**
    ```
    roslaunch vrpn.launch
    ```