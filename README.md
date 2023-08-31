# robart-rest-api-kaercher-rc3
Fork of [Robart MyVacBot REST API](https://github.com/worm-ee/robart-rest-api) to get maximum support on Kärcher RC 3 robot vacuum cleaner.

After Kärcher has dropped ther Home & Garden Classic app I could not controll this robot with my phone. With the knowledge of [Robart MyVacBot REST API](https://github.com/worm-ee/robart-rest-api) I found some http links that run on the Kärcher RC 3, too.

# Http links
If you don't want to use python, simply use these links in your browser or in terminal with e.g. curl
## Get infos
* get robot status

    http://\<robot-ip\>:10009/get/status
* get robot id

    http://\<robot-ip\>:10009/get/robot_id
* get robot schedule

    http://\<robot-ip\>:10009/get/schedule
## Set commands
* send robot home

    http://\<robot-ip\>:10009/set/go_home
* stop robot cleaning

    http://\<robot-ip\>:10009/set/stop
* start or continue cleaning

    http://\<robot-ip\>:10009/clean_start_or_continue?cleaning_parameter_set=1

# Miscellaneous
About the Server on the robot
PORT      STATE SERVICE
10008/tcp open  echo
10009/tcp open  HTTP REST Api
Server: RobArt Custom (0.1)
