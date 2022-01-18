## ROS TOPIC

Dua node yang tadi kita jalankan saling berkomunikasi turtle_teleop_key mengirimkan / mem-publish data dan turtlesim_node *subscribe* ke node publish tersebut. Untuk lebih jelas dalam mengetahui node tersebut, kita dapat menggunakan **rqt_graph**

1. install rqt_graph
   ```
   sudo apt-get install ros-<distro>-rqt
   sudo apt-get install ros-<distro>-rqt-common-plugins
   ```
2. Jalankan roscore dan turtlesim seperti sebelumnya
3. Buka terminal baru, dan jalankan 
   ```
   rosrun rqt_graph rqt_graph
   ```
4. Jika anda melakukan langkah diatas dengan benar, anda akan mendapatkan window baru dengan tampilan berikut
    <img src="http://wiki.ros.org/ROS/Tutorials/UnderstandingTopics?action=AttachFile&do=get&target=rqt_graph_turtle_key.png">
5. Perkenalan perntah rostopic