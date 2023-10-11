<h1>Lab 4: Two-Dimensional Robot Control</h1>
<p>This package reads from the LIDAR lasers on a STDR Simulator robot, feeds it into the subscriber des_vel, and publishes to topic cmd_vel.</p>
<p>It also ensures that the robot does not run into walls by checking the distance to the wall and changing the feed to the publisher.</p>
<h2>Instructions</h2>
<p>Open new terminal and configure ROS</p>
<p>Clone this package and the following package into the src of your workspace</p>
<ul>
<li>https://github.com/cwru-eecs-275/stdr_simulator.git</li>
    <ul>
        <li>This is the STDR Simulator package.</li>
    </ul>
</ul>
<p>Run the following command from the src subdirectory of your workspace.</p>
 <blockquote>roslaunch robot_no_crash simulator.launch</blockquote>
<p>There are two different launch files within the robot_no_crash package</p>
    <ol>
        <li>robot_supervisor.launch starts the robot_no_crash node</li>
        <li>simulator.launch starts the STDR Simulator with the map and the robot, the robot_no_crash node, and the rqt GUI to control the robot.</li>
    </ol>
<p>