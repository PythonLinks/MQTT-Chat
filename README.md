# Review of MQTT Chat Solutions

There are many softwre projects using MQTT for chat.  Here I review the ones which I could find.  Please edit this file. 
 
## Overview of Chat components

A chat application should include a web client, a database, a message broker, an Android client, and an IoS client.  Desktop clients would also be helpful.  Fortunately all of the different pieces exist out there.   We just have to find them, and pull them together.   Here is my high level perspective. 

## Types of chat

There are four types of chat applications. 

1.  **Person-to-person** chat servers are applications like Facebook Messenger, What's App or Signal.  Most of the MQTT chat applications listed here are person-toperson.
2.  **Tech Support Chat is a special case of perston-to-person chat.  It l**ets the anonymous web user chat with a customer service agent.  [LiveChat](http://LiveChat.com) is the best known example.  It supports IP blocking of spammers. 
3.  **Solo Discussion Groups** chats are like Facebook groups, or Twitter Group DMs.  They are all separate from each others. 
4.  **Aggregate Discussion groups** are a collection of closely related chat rooms.  Slack,  Discord and BaseCamp are examples.  
5.  **Topic chat** is where people can chat about a specific topic.  YouTube is the best example.  There is a chat room for every video.  Reddit is also a topic chat server, but it is not real time. 

So here are the applications. 

## [Flutter Client](https://github.com/realdiganta/hitup-messenger)

This is person-to-person chat.  This version runs on IOS, Android, and the web, using the Google Flutter Libraries.   Free and open source. 

## [Applozic](https://www.applozic.com/messaging-api-price.html)

Person-to-person chat.  This is the Rolls Royce Solution. Starting at $149/.month, it includes customizable Android and IoS clients, and every feature imaginable.  They should do what the next guys do, and make it free for the first 1000 users. 

## [MQTT PHP Chat](https://doc.mqtt-chat.com/mqttchat-sdks/setup-and-configuration)

A person-to-person application.  Free for the first 1000 users. Just what every wordpress user needs.  Commercially supported,   

## Topic chat

[This page](https://greenmaps.us/mqtt) supports topic chat.   Every web page is on a different topic, and has its own MQTT chat room.  Use the breadcrumbs in the upper left hand corner of this page to visit the parents, and their topic chat rooms.  If a particular MQTT chat server is of interest to users, I will create a child web page and chat room for it.   MQTT is perfect for this.  One just needs a good database to support it.   I use the  simple topic logger [docker container](https://hub.docker.com/r/pythonlinks/simple-topic-logger).    

So my question is whether anyone else is interested in topic chat?

## [Android Client](https://github.com/jawnpaul/Chatty)

Here is an open source Android client.  Here is a blog posting [part 1](https://medium.com/@jawnpaul) and [part 2.](https://blog.usejournal.com/creating-an-android-chat-app-using-mqtt-part-1-5e543e687380) 

## [IoS Client](https://qiita.com/fuku2014/items/2b8f76c6e60bc9ff14db)

Here is an iOS client for MQTT Chat.  It is written in Japanese, but my girlfriend is Japanese, so we are happy to translate for you.  Here is the Google translate version of the page. 

> I made a chat app for iOS with Swift, so I will introduce it.  
> The source code is also posted, so if you want to make a chat app,  
> I hope it will be helpful for those who are studying Swift.
> 
> What kind of app?  
> The chat app created this time is a very simple app.  
> When you enter the room by entering the room name and user name,  
> It's an app that allows you to chat with other people in the same room.  
> So I don't do user authentication at all.

## [Express Client, Mosca and Mongo DB Server. ](https://github.com/emmanueldg/mqtt-chat)

Here is an open source library for MQTT chat.  

## [Terminal Client](https://www.hackster.io/acellon/terminal-chat-client-8275a7?ref=explore&ref_id=recent___&offset=6)

Here is an MQTT chat client for the terminal, currently running on Raspberry Pi. 

## Android Chat with Auto Discovery. 

Here is a bit of a niche article [about a single chat room shared by multiple android clients](https://www.b4x.com/android/forum/threads/mqtt-chat-with-auto-discovery.75713/), where one acts as the server. 

## Additional Articles. 

[MQTT Chat for Millions of Users](https://medium.com/@rahulbhanushali/mqtt-for-real-time-apps-6e8934b0f818)  In India they built an MQTT app for millions of users.  Perfect for supporting low end devices on low powered networks. 

Here is an article about [how to make your MQTT web chat secure](https://ashleysheaff.com/creating-a-secure-mqtt-web-chat/).
