# Membuat package ROS 1

1. Buat folder untuk package kalian nantinya
   ```
   mkdir -p magang_ros_1/src
   ```
2. Navigasi ke folder src dalam workspace kalian dengan cara
   ```
   cd magang_ros_1/src
   ```
3. Sekarang gunakan command <span style="color:green">catkin_create_pkg</span> untuk membuat package di ROS 1
   ```
   catkin_create_pkg first_pkg std_msgs rospy roscpp
   ```
   Command line diatas akan membuat sebuah package di dalam folder <span style="color:green">src</span> kalian di dalam folder workspace kalian. Command ini juga akan memberikan file <span style="color:red">package.xml</span> serta <span style="color:red">CMakeList.txt</span>
4. Sebelum build package kita, kita perlu melakukan perintah berikut
   ```
   source /opt/ros/kinetic/setup.bash
   ```
5. Untuk membentuk workspace dan menentukan lokasi setup.bash kalian, kalian dapat kembali ke directory folder workspace kalian lalu ketikkan command
   ```
   catkin_make
   ```
6. Jika sukses coba jalanka perintah <span style="color:green">ls</span> pada terminal kalian
   ```
   ls
   ```
   Jika anda melakukannya dengan benar, maka anda akan mendapatkan bahwa dalam folder workspace kalian ada 3 folder, yaitu
        ```
        build,
        devel, dan
        src
        ```
