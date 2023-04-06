> ## Linux Commands
- ls = To see list of files
- cat = To see content in the file
```
cat file1
```
- more = To see content in the file
```
more file1
```
- tail = To see the last few lines of the contet
```
tail file1
```
- tail -f = To see the last few lines of the content and to add the content
```
tail -f file1
```
- locate =  Search for a file or a Directory
```
locate filename
```
- cd = change the directory

- touch = create a file
```
touch file1
```
- mkdir = To create a directory
```
mkdir D1
```
- mv = To move a file from one place to another place
```
mv /home/bharath/linux /home/bharath
```
- rm = To delete a file
```
rm file1
```
- rmdir = To delete a directory
```
rmdir D1
```
- cp = copy a file
```
cp /home/bharath/linux /home/bharath
```
- cp -r = copy files recursively 
```
cd -r /home/bharath/linux /home/bharath
```
- ls -la = To see all the files and directory

- ls -lh = To see size of all file

- sed = Steam editor can be used to perform text editing in a file
```
sed 's/123/456/' file2
```
- find -size = To search for the size of file (find path of the file -size -10c(bytes))

- find -size = To search for the size of file (find path of the file -size -10m(Megabytes))

- find -size = To search for the size of file (find path of the file -size -10k(kilobytes))
```
find -size -/+1M
find -mtine -30
find -name ".php*"
```
- grep = To search any words in number of files at a time
```
grep file README.md
```
- grep -i = To find all variations of a word in a case-insensitive manner
```
grep -i file README.md
```
- du = To see the disk usage of file

- df = To see checking the available and used disk space

- diff = To see the difference between the two files and directory
```
diff file1 file2
```
- wc =  To see number of words, lines and bytes in a file

- wc -l = To see number of lines in a file
```
wc -l file1
```
- zip = To create a zip arcive.zip file
```
zip file1.zip file1
```
- unzip = T unzip archive.zip file
```
unzip file1
```
- ln = To create links between lines



> ## Commands in VI

- Esc = To esc from the terminal
- i = for instert mode
- :wq = To save the data
- :q! = To quit from the file without saveing
- :wq! = To save and quit from the file
- :%s/oldword/newword = To search a word and replace it
- dd = To delete a over all line
- x = To delete a single letter



> ## USER MANAGEMENT

- useradd =  To add user
```
useradd chinna
```
- userdel = To Delete a user
```
userdel chinna
```
- passwd =  To set a password for a user

> ## ACESS MANAGEMENT

- ssh = To establish an SSH connection to a remote machine

- scp = To copy a file securely from one server to another server (scp path of local file username@ip adress:path of remote directory)
```
scp /home/bharath/file1 ubuntu@pvt_ip:/home/bharath/D1
```
- sudo = To execute a command as a root user

- su = To switch user

- chmod = To change permissions for file and Directories
```
chmod 777 file1
```
- chown = To change the ownership of a file or Directory
```
chown chinna file1
```

> ## CONFIGURATION MANAGEMENT

- env = To displays or modifies the environment variables for the current shell session or runs a command with modified environment variables
```
env
```      
- path = To specifies a set of directories where executable programs are located       
- echo = To display text or the value of a variable in the terminal
```
echo 1
```
- export = To set environment variables
```
export MYVAR=hello
```
- hostname = To display or set the name of the current host or system
```
sudo hostname bharath
```
- netstat = To view active network connections, listening ports, and statistics about network traffic
netstat -tulpn
```
-t: Displays TCP connections.
-u: Displays UDP connections.
-l: Displays listening ports.
-p: Shows the process ID (PID) and name that the connection is associated with.
-n: Shows the numeric address and port numbers, rather than resolving them to host and service names.
```
- crontab -e = To create, edit, and manage cron jobs

- crontab -i = To replace the current crontab file with the contents of a new crontab file, after prompting the user for confirmation

- crontab -l = To see thhe list of cronjobs
```
crontab -l
```
- kill : used to terminate a process by using pid
```
kill -9 <1682>
```
- wget : used to downloads file from the internet
```
wget https://dlcdn.apache.org/tomcat/tomcat-10/v10.1.5/bin/apache-tomcat-10.1.5.tar.gz
```
- curl : used to transfer data between servers using various protocols (HTTPS,HTTPS,SCP)
```
curl  -o outputtxt.html https://ubuntu.com/download/desktop.html
```
- ping : used to test the connectivity between two networked devices
```
ping 8.8.8.8
```
- uname : To prints out system information

- history : To prints out the historty of the executed commands

- ps : To displays information about currently running processes

- ps -ux : To view the list of processes running on the system, including their resource utilization and ownership information

- ps -ef : used to view the process tree hierarchy of all processes

- ps -ef | grep <pid> : To view the information about a specific process by its PID



> ## LOG MANAGEMENT

```
- Syslog = A standard protocol used to log messages from different software applications and system services. It is a way to centralize logging   across multiple servers and applications, making it easier to manage and troubleshoot issues.
```
```
- Journalctl = A command-line utility used to query and view logs collected by the systemd journal. It can be used to search for specific log 
  messages, filter logs based on different criteria, and view logs in various formats.
```
```
- Custom logs = It is to refer log messages that are generated by custom applications or scripts. It can contain any type of information, from 
  debug messages to application-specific metrics, and are used to help developers and system administrators monitor and troubleshoot their 
  applications.
```

> ## NETWORK MANAGEMENT

- ifconfig = To display the network configuration of a Linux system's network interfaces

- http = HTTP stands for Hypertext Transfer Protocol, which is a protocol used for transmitting data over the internet. It is a client-server 
  protocol, which means that it is used to send and receive data between a client and a server

- https = HTTPS stands for Hypertext Transfer Protocol Secure, which is a secure version of the HTTP protocol used for transmitting data over
  the internet. HTTPS encrypts the data being transmitted, making it more secure and less susceptible to interception by third parties
															
- Internal Network = An internal network is a network that is used within an organization, typically within a physical location, such as an 
  office or a building. An internal network is usually comprised of multiple devices connected together using switches, routers, and other
  networking equipment. Internal networks are used to facilitate communication between devices within the organization and are often secured
  using firewalls and other security measures to protect against unauthorized access

- External Network = An external network, on the other hand, refers to a network that is outside of the organization's internal network.
  External networks typically refer to the larger internet and other wide area networks (WANs). External networks are used to connect internal
  networks with each other and with the rest of the world. This allows devices on internal networks to communicate with devices on other
  networks and access resources and services that are located outside of the organization's internal networ

- TCP (Transmission Control Protocol) = Is a connection-oriented protocol that establishes a reliable connection between two devices before
  transmitting data. It ensures that all data is transmitted in the correct order and without errors, and uses a variety of error-checking
  mechanisms to ensure the integrity of the data. TCP is commonly used for applications that require a high degree of reliability, such as 
  file transfers, email, and web browsing

- UDP (User Datagram Protocol) = Is a connectionless protocol that does not establish a reliable connection before transmitting data. It does
  not guarantee that data will be transmitted in order or without errors, and does not perform any error checking or retransmission of lost
  data. UDP is commonly used for applications that require low latency and are less sensitive to errors, such as online gaming, streaming
  media, and VoIP (Voice over IP).

- Private Subnet = Range of IP addresses that are reserved for use within a private network, such as a company's internal network. Private
  subnets are not accessible from the internet and are typically assigned non-routable IP addresses, such as those within the ranges of
  10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16. Private subnets are commonly used for internal communication between devices within the
  network and are often protected by a firewall to prevent unauthorized access from external sources

- Public Subnet =  public subnet, on the other hand, is a range of IP addresses that are accessible from the internet and can be used to host
  publicly accessible resources, such as web servers or email servers. Public subnets are typically assigned routable IP addresses, which can
  be accessed from outside the network. Public subnets are commonly used for hosting publicly accessible resources and are often protected by
  security measures such as firewalls, intrusion detection systems, and other security measures to prevent unauthorized access.

- CIDR = (Classless Inter-Domain Routing) notation is a way to represent IP address ranges using a combination of the IP address and a subnet
  mask

- Ports = In computer networking, a port is a logical connection point used by network protocols to enable communication between two devices
  over a network. Ports are identified by a unique number known as the port number, which is used to differentiate between different types of
  network traffic

```
Well-known ports = Port numbers ranging from 0 to 1023, and they are assigned to specific services or applications by the Internet Assigned
                   Numbers Authority (IANA).

Port 80 for HTTP (web traffic)
Port 443 for HTTPS (encrypted web traffic)
Port 25 for SMTP (email)
Port 53 for DNS (Domain Name System)

Dynamic or private ports = Port numbers ranging from 1024 to 65535, and they are used by applications to establish a connection with a remote
                           device. These ports are typically allocated by the operating system or by the application itself, and are used to                               enable communication between two devices
```

- Application = Software program that is designed to provide a platform for hosting and running applications or websites on a networ.                           These servers are used to manage and distribute web-based applications, dynamic web pages, and other content over the                           internet or an internal network

- Web Server = designed specifically for hosting and serving web pages and other web-based content. Web servers respond to HTTP requests from
               clients (typically web browsers) and return HTML pages, images, and other media files. Examples of web servers include Apache,
               Nginx, and Microsoft IIS

- Load balancing = The process of distributing network traffic across multiple servers to ensure that no single server is overloaded or
                   becomes a single point of failure. Load balancing is typically used in web applications, where large numbers of clients
                   are accessing the same resources, such as web pages or APIs.

- High availability (HA) = Is a system design approach that aims to ensure that a system or service remains operational and accessible to users                            at all times, even in the event of hardware, software, or network failures. High availability is achieved through
                           redundancy and failover mechanisms that ensure that a backup system or service can take over if the primary
                           system fails

> ## SHELL SCRIPT TO INSTALL APPICATION SERVERS AND PROXY TOOLS

- Update your system's package index 

```
sudo apt-get update
```
- Install Java on your system. Tomcat requires Java to run

```
sudo apt-get install default-jdk
```
- Download the latest version of Tomcat from the official Apache Tomcat website with wget
```
wget https://dlcdn.apache.org/tomcat/tomcat-10/v10.1.7/bin/apache-tomcat-10.1.7.tar.gz
```
- Extract the downloaded file using the tar
```
tar apache-tomcat-10.1.7.tar.gz
```
- Move the extracted Tomcat directory to a location of your choice
```
sudo mv apache-tomcat-10.1.7 /opt/tomcat
```
- Set the CATALINA_HOME environment variable to point to the Tomcat installation directory
```
export CATALINA_HOME=/opt/tomcat
```
- Start Tomcat by running the following command
```
$CATALINA_HOME/bin/startup.sh
```

> ## CONFIGURATION OF APPLICATION SERVER

- Edit the tomcat.service file and replace the content
```
[Unit]
Description=Tomcat
After=network.target
[Service]
Type=forking

User=tomcat
Group=tomcat

Environment="JAVA_HOME=/usr/lib/jvm/java-1.11.0-openjdk-amd64"
Environment="JAVA_OPTS=-Djava.security.egd=file:///dev/urandom"
Environment="CATALINA_BASE=/opt/tomcat"
Environment="CATALINA_HOME=/opt/tomcat"
Environment="CATALINA_PID=/opt/tomcat/temp/tomcat.pid"
Environment="CATALINA_OPTS=-Xms512M -Xmx1024M -server -XX:+UseParallelGC"

ExecStart="/opt/tomcat/bin/startup.sh"
ExecStop="/opt/tomcat/bin/shutdown.sh"

[Install]
WantedBy=multi-user.target
```
- systemctl daemon-reload
- systemctl start tomcat
- systemctl enable tomcat

- Now edit tomcat-user.xml file in this path /opt/tomcat/conf/tomcat-users.xml
```
<role rolename="manager-gui"/>
  <role rolename="manager-script"/>
  <user username="tomcat" password="admin123" roles="manager-gui,manager-script"/>
  </tomcat-users>
```
-Now edit  META-INF file in this path /opt/tomcat/webapps/manager/META-INF/
```
<?xml version="1.0" encoding="UTF-8"?>
<!--
  Licensed to the Apache Software Foundation (ASF) under one or more
  contributor license agreements.  See the NOTICE file distributed with
  this work for additional information regarding copyright ownership.
  The ASF licenses this file to You under the Apache License, Version 2.0
  (the "License"); you may not use this file except in compliance with
  the License.  You may obtain a copy of the License at
http://www.apache.org/licenses/LICENSE-2.0
  Unless required by applicable law or agreed to in writing, software
  distributed under the License is distributed on an "AS IS" BASIS,
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
-->
<Context antiResourceLocking="false" privileged="true" >
  <CookieProcessor className="org.apache.tomcat.util.http.Rfc6265CookieProcessor"
                   sameSiteCookies="strict" />
<!--  <Valve className="org.apache.catalina.valves.RemoteAddrValve"
         allow="127\.\d+\.\d+\.\d+|::1|0:0:0:0:0:0:0:1" />
<Manager sessionAttributeValueClassNameFilter="java\.lang\.(?:Boolean|Integer|Long|Number|String)|org\.apache\.catalina\.filters\.CsrfPreventionFilter\$LruCache(?:\$1)?|java\.util\.(?:Linked)?HashMap"/> -->
</Context>
```
- systemctl restart tomcat

- Installation of apache
```
sudo apt install apache2
````
- Then enable and start the Apache service 
```
sudo systemctl enable apache2
````
- Then start the Apache
```
sudo systemctl start apache2
```
- Create an index file for Application server
```
echo "<H1>Hello! This is webserver1: ip adress </H1>" | sudo tee /var/www/html/index.html
```
- If a firewall is running on your system, you will need to allow Apache traffic
```
sudo ufw allow 80/tcp
```
- Then reload the firewall configurations
```
ufw reload
```
Now try accessing the site in your web browser
```
http:// ipadress
```


> ## INSTALLATION AND CONFIGIUARION OF HAPROXY

- On haproxy server edit /etc/hosts file and add application server ip adress
```
sudo vi /etc/hosts
```
- installation of haproxy
```
sudo apt-get update
sudo apt-get upgrade
sudo sudo apt install haproxy
```
- Configuration of haproxy as a load balancer

- Edit the /etc/haproxy/haproxy.cfg file
```
sudo vi etc/haproxy/haproxy.cfg

```
- Add this Text with your Application server ipadress 
```
frontend haproxy_in
        bind *:80
        mode http
        default_backend haproxy_http

backend haproxy_http
        balance roundrobin
        mode http
        server servera 172.31.49.93:80 check
```

- Now restart haproxy 
```
sudo systemctl restart haproxy.service
```
- Now check the status of the haproxy
```
sudo systemctl status haproxy.service
```
- Now start the haproxy
```
sudo systemctl start haproxy.service
```
- Now open haproxy in browser
```
http://ipadress
```













 
