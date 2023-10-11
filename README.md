<h1>Lab 4: Two-Dimensional Robot Control</h1>
<p>This package reads from the LIDAR lasers on a STDR Simulator robot, feeds it into the subscriber des_vel, and publishes to topic cmd_vel.</p>
<p>It also ensures that the robot does not run into walls by checking the distance to the wall and changing the feed to the publisher.</p>
<h2>Instructions</h2>
<p>Open new terminal and configure ROS</p>
<p>Clone the following package</p>
<ul>
<li>https://github.com/cwru-eecs-275/stdr_simulator.git</li>
    <ul>
        <li>This is the STDR Simulator package.</li>
    </ul>
</ul>
<p>Set up a catkin workspace and clone this robot_no_crash package into the src subdirectory.</p>
<p>There are two different launch files within the robot_no_crash package</p>
    <ol>
        <li>robot_supervisor.launch starts the robot_no_crash node</li>
        <li>robot.launch starts the STDR Simulator with the map and the robot, the robot_no_crash node, and the rqt GUI to control the robot.</li>
    </ol>
<p>
<p>Edit the robot.launch file and ensure the path of the include file has /home/< your-username >/ ... </p>
<p>Run the following two commands from the workspace.</p>
 <blockquote>
     roslaunch robot_no_crash robot.launch
     rqt
 </blockquote>
