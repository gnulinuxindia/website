---
title: "Get an IRC Bouncer"
date: 2021-12-21T17:45:51+05:30
draft: false
---

IRC stands for Internet Relay Chat and is one of the oldest chat protocols.
Its primarily used for group chats, but also has support for one on one chats.

IRC servers usually don't store the messages that are being sent. They transmit
messages directly from the sender to the receiver. So if the sender is not
connected to the IRC server then they won't be able to receive messages.

To surpass this you can make use of an IRC bouncer. As the name suggests its a
server that will receive messages for you and bounce it over to you when you
are online again.


You could ask for a bouncer in any of our
[group chats]({{< relref "welcome.md" >}})
and the admins will make a
you bouncer account for you at [znc.gnulinuxindia.org](https://znc.gnulinuxindia.org).



## Instructions

- Once you receive the login details from the admins you can log into
  [znc.gnulinuxindia.org](https://znc.gnulinuxindia.org)
  and change your password

- Go to `Your Settings` tab under `webadmin`.

- Change your ZNC password from the `Authentication` panel.

- To get started we need to first let your bouncer account connect to a network
  (an IRC server like libera) and then you should connect your IRC client to 
  gnulinuxindia.org at port 1079 with the your ZNC username.

  ```
  Your Client ----->  gnulinuxindia.org ------> network (eg chat.libera.net)
            ZNC username              IRC username
  ```
- Add a network from the `network` panel. Once created the network panel will display the format of password that needs to be used to connect to that network through the bouncer.

- You could connect with the your IRC client with these parameters
  
  ```
  username: <znc_username>
  password: <znc_username>/<network_name>:<znc_password>
  host: gnulinuxindia.org
  port: 1079
  ```

