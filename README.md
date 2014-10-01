Rader
=====

RSS Reader on MQTT service

- pub/sub portion is implemented by MQTT broker
- feed data model for each client is implemented by process on Erlang
  - cached on browser
  - tail N from process to re-draw UI
  - sort via Social data (ego searched on Twitter etc.)
    - Token bearer is the process
    - process behaviour can be described by DSL(Lua)
  - filter out 'READ' items on social network
  - ask someone to read, or mention count on your timeline
- broke down to microservices to support social activities.

Repository
+ main > marshaller (everything)
+ customer specific 
+ API


Crawler
+ publisher
+ get diff from previous sampling
+ API


Client / iOS App, Facebook App, browser App 

+ multi-subscriber

+ view latest
+ social activities
  - comment
  


Web Service

+ store Social data
+ unread data control

Agents

+ MQTT re-publisher
+ IRC bot with template
+ Twitter bot

