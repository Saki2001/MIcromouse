This is a bot that is created in URDF and simulated in Gazebo that can detect walls and try to move without hitting the walls.

Plugins Used:

Differential Drive Plugin : This plugin is used to publish the velocity of the bot in terms of both linear and angular to the "/cmd_vel" topic which is used to move the bot linearly as well as in rotation also. This plugin also needs the data of the amount of torque that is to be given to the wheels of the bot, distance between the wheels, also the links to which the torque is to be applied.

Gazebo Ros GPU Laser : This plugin is used to publish the distances of objects from the GPU Laser sensor to the topic "/scan_top" and we need to subscribe to the topic to recieve the distances.
