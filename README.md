# Line-Follower
Arduino Code for running a line follower on a track marked with black lines

forward(), back() are functions to move the bot forward.
hard_left() and hard_right() move the bot left or right without moving the bot forward (therefore a hard left or right).
soft_left() and soft_right() move the bot left or right with some forward velocity too

velocity() function can be used to move the motor by assigning values to the two motors

The main function contains the code to drive the bot on the black line in the middle of the white background. 
A PD controller has been used to keep the bot moving on the track. pd = Kp * (error) + Kd * (error - previous error).
Compare this value with a threshold and assign a velocity to the motors as given in the code by using some suitable thresholds (thresh1 and thresh2) which depend on your bot's hardware.
