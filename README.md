# first-project
To install the rose system, we need 3 steps The first step is to download the virtualBox
https://www.virtualbox.org/wiki/Downloads
I chose the Mac version
We install with it the Extension Pack
Step Two: Install Ubuntu on VirtualBox
https://ubuntu.com/desktop
I downloaded version 20.4
I opened virtualBox, I clicked on the new button, typed the name ubuntu, the type of system Linux, then clicked next, then specified the size of memory, then clicked on next, chose create virtual hard disk now, then clicked create Choose the virtual machine disk, then the storage we choose the dynamically allocated, then the next and then create and then click on the settings button click on storage go to empty we choose choose a disk file click download choose unbent click ok click start Choose Ubuntu click start Choose the English language install Ubuntu Choose the keyboard language English Click continue install now I filled in the data Name Anfal Password a123a123 Click on continue Wait for the installation to complete and then press restart now It will restart the device and enter Ubuntu immediately after typing the password
Step Three: Install ros on Ubuntu
open terminal Write
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
sudo apt install curl # if you haven't already installed curl
  
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add –
sudo apt-get update
(((((It takes some time))))))
sudo apt-get install ros-kinetic-desktop-full
echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc source ~/.bashrc
sudo apt install python-rosdep python-rosinstall python-rosinstall- generator python-wstool build-essential
sudo apt install python-rosdep sudo rosdep init
rosdep update
roscore
 
