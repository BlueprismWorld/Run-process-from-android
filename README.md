# Run-process-from-android
Run BP processes from android application.<br><br>
This application is developed based on [Link](https://bpdocs.blueprism.com/bp-6-9/en-us/helpResourcePCCommands.htm?tocpath=Interface%7CAdvanced%20options%7C_____4 "BP Resource pc commands").

# Screenshots.
<div align="center">
  <img src="Screenshots/Screenshot_2022-01-12-22-10-15-964_com.bpcontrolroom.nk.jpg" width="170px" height="360px"</img> 
    <img src="Screenshots/Screenshot_2022-01-12-21-08-38-106_com.bpcontrolroom.nk.jpg" width="170px" height="360px"</img> 
    <img src="Screenshots/Screenshot_2022-01-12-21-09-31-032_com.bpcontrolroom.nk.jpg" width="170px" height="360px"</img> 
  <img src="Screenshots/Screenshot_2022-01-12-21-09-50-437_com.bpcontrolroom.nk.jpg" width="170px" height="360px"</img> 
  <img src="Screenshots/Screenshot_2022-01-12-21-10-34-138_com.bpcontrolroom.nk.jpg" width="170px" height="360px"</img> 
   
</div>

# Features #
Run processes remotely.<br>
Manage sessions remotely.<br>
Send startup parameters and session variables rempotely.<br>
Filter processes and sessions.<br>
No ads<br>


# Prerequisites
Make sure Runtime resource pc and android device both in same network(alternatively use ngrok port forwarding for outside network).
Make sure the target resource pc is running like below.<br>
![picture alt](Screenshots/resourcepc.png "Runtime resource")
<br><br>
Make sure under system tab "Session management enforces permissions of controlling user" option is diabled like below
<br><br>
![picture alt](Screenshots/session.png "permission")
<br>
# How to login.
Server Url : enter target resource pc ip address and port no(default port no is 8181)<br>
Ex: if target resource pc ip is 192.168.102.102<br>
<b>http://192.168.102.102:8181</b><br>
Username & Password will be Blueprism username password.
<br>
# How to set startup prameters.
In process tab select process and click on down arrow then enter startup parama in input field in below format.<br>
<b>Param Name,type,value</b><br>
if you have more than one startup params you can enter seaparated by semicolon(;) like below<br>
<b>Param name,type,value;Param name,type,value;and so on...</b>
# How to send session variables.
As soon as you run the process session will create under sessions tab automatically, if process is having session variables automatically it will appear in session tab and under value you can change and click "sesnd session variable" button, if succesfully sent or not you will get confirmation popup, And also you can check current value of session variable by clicking "Get S Vars" button. 
# How to stop process.
Under session tab by using "stop" button stop the process(this will perform request stop make sure in process IsStopRequested() is implemented then only the process will stop).

#  #
If you found any bugs please mail to naveen.rpa93@gmail.com.
