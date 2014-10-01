Rader
=====

RSS 'Social' Reader on MQTT bound services

- pub/sub portion is implemented by MQTT broker
- feed data model for each client is implemented by process on Erlang
  - cached on browser
  - tail N from process to re-draw UI
  - sort via Social data (ego searched on Twitter etc.)
    - Token bearer is the process
    - process behaviour can be described by DSL(Lua)
  - filter out 'READ' items on social network
  - ask someone what to read, or mention count on your timeline
- broke down to microservices to support social activities.
- to make money
	- insert ad
		- affiriate by RT (curator is rewarded)

Repository
=====

+ main > marshaller (everything)
	- Map/Reduce to extract social data
+ customer specific 
+ API for 


Crawler
======

+ publisher
+ get diff from previous sampling
+ API (for supervisor)
	- set entry (RSS_URL)
	- purge RSS (if no subscribing user exists, crawling stop)
	- rotate RSS entries


Client / iOS App, Facebook App, browser App 
=======

+ multi-subscriber

+ view latest
+ social activities
  - comment
  - recommend (RT, cite, etc.)
  


Web Service
=====

+ store Social data
+ unread data control

Agents
=====

+ MQTT re-publisher
+ IRC bot with template
+ Twitter bot