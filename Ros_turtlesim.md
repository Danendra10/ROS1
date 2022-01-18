# Turtle Sim di ROS 1
1. Pastikan roscore sudah berjalan dengan perintah
   ```
   roscore
   ```
2. Buka terminal baru, lalu source ke setup.bash seperti pada langkah sebelumnya
   ```
   source /opt/ros/(nama distro)/setup.bash
   ```
3. Jalankan turtlesim dengan
   ```
   rosrun turtlesim turtlesim_node
   ```
4. Selamat!!! Sekarang anda dapat bermain dengan turtle sim, akan tetapi anda belum dapat menggerakkannya bukan? untuk melakukannya, gunakan perintah berikut
   ```
   rosrun turtlesim turtle_teleop_key
   ```
5. Jika anda selesai, anda dapat terminate dengan tombol <span style="color:green "> ctrl + c </span>
6. Selanjuya, kita akan melanjutkan ke ROS TOPIC