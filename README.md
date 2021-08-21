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
  <h3> Setting up SSH keys</h3>
  <p>To use Gazebo, you will need to have a GitHub account. The installation scripts require a GitHub account with an SSH key.</p>
  <h4>To create an SSH key, run the following in a terminal:<h4>
    <li>ssh-keygen</li>
    <li>sudo apt install xclip git</li>
   <li>xclip -sel clip < ~/.ssh/id_rsa.pub</li>
     <h4>Adding your SSH key to GitHub</h4>
     <p>  Next, you'll want to install xclip. This program will allow you to copy the contents of the id_rsa.pub file to your clipboard so you can paste it into GitHub. To install xclip, run the following command:  
$ sudo apt install xclip git
Once you've installed xclip, you need to copy the id_rsa.pub file to your clipboard. To do so, run the following command:
$ xclip -sel clip < ~/.ssh/id_rsa.pub
Adding your SSH key to GitHub
Now, log into your GitHub account and paste your SSH key. The SSH key field is located in your account settings under "SSH and GPG keys". Add a new SSH key by pressing "New SSH key" and pasting your SSH key in the box. Make sure to give it a name!</p>
       
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
