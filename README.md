## Ezbob asessment
there is only endpoint of application:[POST] http://localhost:8081?number=10 

number in range 1-1000

Explanation:

for log requests I decided to use spring Actuator because this is common problem and
 there is no need to invent custom implementation to solve it
 
 Spring Actuator intercept all POST requests in CustomTraceRepository class and send it to service-log asynchronously 
 
 To generate array of shuffled numbers i created array which start with 1 and and with N
 after I shuffle it with O(N-1) time complexity
 
  
 
