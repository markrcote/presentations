Abstract
========

Advice on how to design and implement networking code for use in automation: learn how sockets work, plan for and handle errors, and design effective protocols.

Outline
=======

Automation and network programming
----------------------------------

Controlling a remote device via network is not an uncommon automation task. Automation developers, however, tend to be generalists and may not have in-depth knowledge or experience in network programming. We will cover some socket fundamentals and general protocol design to make sure you get off to a good start.

Learn how sockets work
----------------------

Sockets are complicated, but there are some basic concepts that are essential: the difference between blocking and nonblocking and which to use, how to handle timeouts and determine if and how a connection has closed, and when and how data is (or should be) buffered.

Plan for and handle errors
--------------------------

Devices will fail and software will crash, and automation software has to be ready to cope to avoid adding noise to test results and to provide clear indications of real errors. Failures can occur at the connection, action, and user layers, and each should have their own way to handle them.

Design a robust, generic protocol
---------------------------------

Your automation needs should dictate the basics of your protocol. A line-terminated protocol is simple but limited--it may need more structure if you need to to transfer raw data. Abstract away as much as possible from the underlying OS of the remote device and concentrate on what information and actions are necessary for automation.

