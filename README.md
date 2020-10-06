# Ezbob asessment
### Project structure
project consist of three repoository:

https://github.com/3620849/ezbob-discovery

https://github.com/3620849/ezbob-service-shuffle

https://github.com/3620849/ezbob-service-log

###USE
there is only endpoint of application:[POST] http://localhost:8081?number=10 

number in range 1-1000

###TO LOG:

To log requests I decided to use spring Actuator because this is common problem and
 there is no need to invent custom implementation like create filters to solve it
 
Spring Actuator intercept all POST requests in CustomTraceRepository class and send it to service-log asynchronously 

###Shuffle Array 
To generate array of shuffled numbers i created array which start with 1 and and with N
 after I shuffle it with O(N-1) time complexity
 
###Validation
To validate requset i used spring validation starter, request with wrong range will return to user response with message and status 400 BAD REQUEST
 
  
 
