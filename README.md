# Robotics_Project4
This is a demonstration of a SLAM approach by using the rtabmap ROS package

To execute the Project:

1. Clone the Repository Folder "Robotics_Project4" to your /home/<user> directory
2. Enter to the folder:
	cd ~/Robotics_Project4/
  
3. Compile the Workspace by using the script provided:
	./compile_all
 
4. Open 3 terminals.
	4.1. First Terminal: 
  		cd ~/Robotics_Project4/
	      	source devel/setup.bash
	       	roslaunch my_robot world.launch
	or
		./robot
	
	4.2. Second Terminal:
	       	cd ~/Robotics_Project3/
	      	source devel/setup.bash
	      	roslaunch my_robot mapping.launch
		or
		./mapping
  
	4.3. Third Terminal:
        		cd ~/Robotics_Project4/	
		source devel/setup.bash
      		roslaunch teleop_twist_keyboard teleop.launch
		or
		./teleop
		or
		rosrun teleop_twist_keyboard teleop_twist_keyboard.py
  

5. Move the robot by using the keys indicatd by teleop_twist_keyboard.

6. When finish, open the downloaded database file and copy it to ~/.ros directory, then
	rtabmap-databaseViewer ../.ros/rtabmap.db
	or
	./open_database	

7. To close everything:
	cd ~/Robotics_Project4/
	./pkill_all


