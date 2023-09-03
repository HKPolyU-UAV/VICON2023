# Some Remote Tricks

## SSH - to interact with remote computers
1. **ssh**

    Install SSH
   ```
   sudo apt-get install openssh-server
   ```

2. **Do ssh**

    ```
    ssh {username}@{ip_addr} -p {port_number} # note that port_number is required for DOCKER
    ```
3. **VScode**
    
    Refer to [here](https://github.com/HKPolyU-UAV/useful_tools/blob/main/vscode_github/vscode_github.md#remote-ssh) for more.

## Transporting Files - to send files thru ssh
    Just create a shell script for the following:
    ```
    sudo scp -P {port_number} {file_name} {username}@{IP_ADDR}:{directory_localtion}

    # if you want to send a folder, can do the following first
    zip -r {filename}.zip {filename}
    ```

    Note that {port_number} is usually 22 or 6666 for ssh in our lab.
