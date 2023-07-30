# Template for ROS2 projects

Template for docker based development environment for <a href="https://www.ros.org/">ROS2</a> projects including the <a href="https://vulcanexus.org/" target=_blank>Vulcanexus</a> installation.<br>
It allows usage and development of programs with an UI and works on a Linux or Windows host.<br>
It has no implemented compose file for MacOS!
<p>
The template uses docker compose to startup the container(s).<br>
The included Dockerfile bases on the image "iron-full" provided in <a href="https://hub.docker.com/r/stepkun/vulcanexus" target=_blank> docker hub</a> and 
created by <a href="https://github.com/stepkun/dockerfiles/tree/main/vulcanexus" target=_blank>ROS2/Vulcanexus image</a>
<p>
Template should work on amd64 and arm64 architectures.<br>
It should work with any image for ROS2.
<p>
The inspiration for this comes from <a href="https://www.allisonthackston.com/articles/vscode-docker-ros2.html">Allison Thackston</a> and her <a href="https://github.com/athackst/vscode_ros2_workspace">template</a>, so all credits goto her.
