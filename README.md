# class-197
`FTP severs and troubleshooting`

-Creating FTP server and client -FTP commands
we are going to learn how to set up a server and client
Server is used to store the files so that multiple users can access these files.

Servers can be local such as a home server where only you and your family members can use that. But we can have an online server where anyone on the internet can connect

a server is just a computer, where we store files, so that multiple users can access these files. servers are designed to have a lot of memory and they are very fast as well. ex: youtube(billions of videos uploaded and anyone can watch the videos and upload videos on youtube)
what you can do is create a server using your computer?

This computer will have its IP address and all the people who are on your network will be able to access these files on their devices. Because the server and the devices are connected using a cable connection or Wifi connection they can transfer the files at a very high speed.

This is possible because all the files are present at a server. Other devices or clients can connect with the server and access files. This happens using FTP or File Transfer protocol.
In a local server, Only those people can access the file which are connected to your wifi or network. No one outside your network can access these files. These types of servers are made in schools, banks, hospitals, govt offices, where security is most important.

but if you want to make a website and upload videos on the website so that people around the world can see those videos then we need to create a server in a way so that anyone on the internet can see these videos. You must have seen a godaddy ad on youtube or TV, have you seen it? Godaddy provides the hosting for the website, where they basically provide their own server and our website is stored on their server. Our website has an IP address. Using that IP address anyone can access the website.

create a very simple Server and client arrangement using Cisco packet tracer and we will see how we can transfer files from a server to a client computer using FTP.

We need 3 components,

--first we need a server.On the server we will store our files. --Then we need a switch.we want to connect multiple devices with the server and switch will provide us ports for that. -At last we need clients.Client is nothing but a normal PC or a laptop. We can have multiple clients with the server.

-server -PT-Switch for this Activity -pc

use copper straight through cable to connect all 3 devices. Select the copper straight through cable and click on the server and select the fastethernet port then click on the Switch and select the fast ethernet port.Next step is to connect the switch with the computer. For this also we are going to use copper straight through cable.
Our cable connections are complete. Now we need to do few important steps such as: ● Assigning IP address to Computer and server. ● Creating user and password for the server. ● Run FTP commands
server ip 192.168.1.1 set the username and password for the server. Because you don’t want anyone to login to the server and access the files. double click on the server and select the services tab. On the left hand menu click on the FTP. here a page will open where we can set username and password.

admin admin

give permissions like (read,write,delete ,....check the checkboxes) write-user can add the files to the server and create new files. read- user can read the files from the server. delete= user can delete the files from the server. rename- user can rename the file And at last list- user can list down or see all the files present in the server.
Remember the username and password, because it is going to be used while accessing the files from the server

Click on the add button and you will be able to see that the user has been created.
set the ip of computer

Here we need to set 2 things, one is the IP address and then the default gateway. Which is going to be the IP address of the Server.

ftp 192.168.1.1 (server ip)

give id,pwd of server

dir

help

get xyz.bin

rename xyz.bin test.bin
------------------------------------------------------------------------------------------------------------------------------------------------
quit

swtich with 3 computer s(troubleshooting)

First step is to check the IP address. Go to the each computer and check if the PC is assigned an IP or not. Next step is to check the cable connection. To connect the switch and the PC we use copper straight through cable. The cable looks correct because we can see the green triangles on the connections. When we first perform a ping between 2 computers which are connected through a switch. Then the switch stores

show mac-address-table: To get the mac addess of the computers connected to switch; It works in switch only.
