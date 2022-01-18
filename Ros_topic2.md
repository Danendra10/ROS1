# Perkenalan rostopic

1. Untuk melihat perintah yang ada, anda dapat melakukan
   ```
   rostopic -h
   ```
   Maka anda akan mendapatkan output seperti berikut<br/>
    ```
    rostopic bw     display bandwidth used by topic
    rostopic echo   print messages to screen
    rostopic hz     display publishing rate of topic    
    rostopic list   print information about active topics
    rostopic pub    publish data to topic
    rostopic type   print topic type
    ```
## **ROSTOPIC ECHO**
1. Selanjutnya mari kita lihat apa itu rostopic echo<br/>
   Saat kita menjalankan perintah <span style="color:green">rostopic echo</span>, kita akan mendapatkan data apa saja yang dipublish oleh topic tersebut. Anda dapat menjalankan perintah ini dengan cara:
   ```
   rostopic echo [nama topic]
   ```
2. Mari kita coba pada topic turtlesim kita di tutorial sebelumnya, pada terminal baru, ketikkan:
   ```
   rostopic echo /turtle1/cmd_vel
   ```
   Anda akan mendapatkan output berupa nilai nilai yang dikirimkan oleh topic tersebut <br/>
   <br/>
   Sekarang coba anda refresh graph kalian, maka akan ada node baru yang subscribe ke node /teleop_turtle
   <img src="http://wiki.ros.org/ROS/Tutorials/UnderstandingTopics?action=AttachFile&do=get&target=rqt_graph_echo.png">
## Untuk lengkapnya anda dapat membaca [disini](http://wiki.ros.org/ROS/Tutorials/UnderstandingTopics)