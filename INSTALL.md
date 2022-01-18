# Install ROS NOETIC on UBUNTU
___

1. Konfiguarsikan Repo Ubuntu
    ``` 
    sudo apt-get-repository universe
    sudo apt-get-repository multiverse
    sudo apt-get-repository restricted
    ```
    Lengkapnya anda dapat membaca [disini](https://help.ubuntu.com/community/Repositories/Ubuntu)

2. Setup komputer untuk menerima perangkat lunak dari packages.ros.org
   ``` 
   sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
    ```
3. Setup Key
    ```
    sudo apt install curl # if you haven't already installed curl

    curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
    ```
4. Instalasi

    a. Pastikan package up to date
    ```
    sudo apt update
    ```
    b. Install ROS full
    ```
    sudo apt install ros-noetic-desktop-full
    ```
    c. Jika anda ingin menambahkan package sendiri, anda dapat menggunakan
    ```
    sudo apt install ros-noetic-(NAMA PACKAGE)
    ```
    Anda dapat mencari package [disini](https://index.ros.org/packages/page/1/time/#noetic)
    
    Atau anda dapat menggunakan perintah
    ```
    apt search ros-noetic
    ```

5. Environment Setup
    
    Anda harus memanggil ini di setiap terminal bash ROS anda
    ```
    echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
    source ~/.bashrc
    ```

6. Install *Dependencies*

    ```
    sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
    ```

    ```
    sudo apt install python3-rosdep
    sudo rosdep init
    rosdep update
    ```

#### Anda dapat melihat video tutorial [berikut]() untuk lebih jelasnya