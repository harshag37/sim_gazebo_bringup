<h1>Introduction to Gazebo </h1>
<div class="gazebo">
<h3 display: block;>WHY GAZEBO?</h3>
<p align="center">
</br><img src="https://gblobscdn.gitbook.com/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXaIxqcmP2grIz5ToTW%2F-MXaND_w1UbqoGHP4VNv%2Fgazebo.png?alt=media&token=a05f7459-89f1-454a-a581-59ea9da22411" width="687" height="319"> 
</p>
<p>Gazebo is a full-fledged simulation environment that is compatible with PX4. In 2021, NXP Cup contestants may use the Gazebo simulation for an extra challenge at home. The benefit to using the Gazebo simulation environment is that you can test your code without crashing or damaging your actual NXP Cup car. The code modules that you run on your actual NXP Cup car can be ported to the Gazebo simulation environment with ease - and if you're using a brushless Cup car, you'll essentially be running the same exact code.<p>
</div>
<div class="installation">
<h3 display: block;>Installing ROS2</h3>
<h4>You need to download this file inorder to install the ROS</h4>
<a href="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXcfaeFblmznqth_0fk%2F-MXcgSRrBPzq5-K6O-C5%2Ffoxy_install_aim.sh?alt=media&token=2adf3a55-8463-4ff1-890e-67b6d32fe747">Click here to download</a>
  <h5>RUN THE FOLLOWING COMMANDS</h5>
<ul display: block; style="font-family:verdana">
  <li>cd ~/Downloads</li>
  <li>chmod a+x foxy_install_aim.sh</li>
  <li>./foxy_install_aim.sh</li>
  <li>source ~/.bashrc</li>
</ul>
</div>
<div class="robocon">
<h3 display: block;>Installing Robocon Gazebo</h3>
 <ul display:block;style="font-family:verdana">
    <li>cd ~</li>
    <li>mkdir -p robocon_ws/src && cd robocon_ws/src</li>
    <li>git clone https://github.com/harshag37/sim_gazebo_bringup.git</li>
    <li>cd ~/robocon_ws</li>
    <li>colcon build --packages-select sim_gazebo_bringup --symlink-install</li>
    <li>echo "source /home/$USER/robocon_ws/install/setup.bash" >> ~/.bashrc</li>
    <li>source ~/.bashrc</li>
    <li>ros2 launch sim_gazebo_bringup sim_gazebo.launch.py</li>
   </ul>
</div>
