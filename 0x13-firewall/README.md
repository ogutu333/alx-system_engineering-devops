INTRODUCTION.

A Firewall is a network security device that monitors and filters incoming and outgoing network traffic based on an organization’s previously established security policies. At its most basic, a firewall is essentially the barrier that sits between a private internal network and the public Internet. A firewall’s main purpose is to allow non-threatening traffic in and to keep dangerous traffic out.

TASKS.

0-block_all_incoming_traffic_but - Install the ufw firewall and setup a few rules on web-01.

Configure ufw so that it blocks all incoming traffic, except the following TCP ports:
-22 (SSH)
-443 (HTTPS SSL)
-80 (HTTP)

100-port_forwarding - Configure web-01 so that its firewall redirects port 8080/TCP to port 80/TCP.

Terminal in web-01;
-My web server nginx is only listening on port 80
-netstat shows that nothing is listening on 8080

