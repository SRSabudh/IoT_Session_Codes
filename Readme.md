This file is related to IoT with cloud baiscs session in sabudh by
Saurabh Ritu.   
    
Hey Folks, you all have gone through the session and know the basics concepts of mosquitto, mqtt and esp32 and paho python client.
So, I want from all of you guys to implement the session setup into your local machine (laptops) and do some interesting stuff from your own ideas.

First you need to install mosquitto on your system.

\*\> esp32 client code :- it is used to send data to mosquitto broker on
a particular topic

\*\> mqtt\_data\_dumper\_cvs.py :- it is a python code used to subscribe
to a particular topic, fetch data and store it in csv file format / or
anything up to you.

\*\> visualization\_basic :- this python code is used to visulaize the
real-time data in graph using matplotlib & its FuncaAnimation feature.

\*\> Basic Operation on Mosquitto:-

    #> Set up mosquitto Broker ( with and without -c & -v flags ) [ mymosquitto.conf is your custom configuration file ]
        => mosquitto -c mymosquitto.conf -v

    #> Publish Msg to a topic
        => mosquitto_pub -h localhost -m "on" -t home/myroom/sidebulb

    #> Subscribe to the topic 
        => mosquitto_sub -h localhost -t home/myroom/sidebulb

\*\> Note:- you have to downoad paho library from pip before using it
inside python, Use:- pip install paho-mqtt.

    Link More about PubSubClient :- https://pubsubclient.knolleary.net/api#PubSubClient

    Link Mosquitto :- https://mosquitto.org/download/   
        
 ![Mini IoT frmaework@1 25x](https://user-images.githubusercontent.com/97020522/171807801-6cd1974e-c85c-48e9-824f-31fd1f7a3506.png)

