OpenRSTP_VS2013
===============

It is base on liveMedia OpenRTSP and add VS2013 related project and solution for implement.
(liveMedia http://www.live555.com/liveMedia/)

All code base on liveMedia, I just add solution and project setting for who want to implement via Visual Studio 2013.
Here is detail step which could help you do the same thing. The reason I choose meida server is because it is must easy to verify whole detail. Let me know if any question.

###To Setup with VS2013 for OpenRTSP MediaServer
-	liveMedia
  - Open Project Win32 Console -> Static Library
    -	uncheck "Precompiled header" and "Security Development Lifecycle (SDL) checks"
    -	Include all cpp and .hh
  -	Add include as follow:
    -	../include
    -	../../groupsock/include
    -	../../UsageEnvironment/include
-	groupsock 
  - Open Project Win32 Console -> Static Library
    -	uncheck "Precompiled header" and "Security Development Lifecycle (SDL) checks"
    -	Include all cpp and .hh
  -	Add include as follow:
    -	../include
    -	../../UsageEnvironment/include
-	BasicUsageEnvironment 
  - Open Project Win32 Console -> Static Library
    -	uncheck "Precompiled header" and "Security Development Lifecycle (SDL) checks"
    -	Include all cpp and .hh
  -	Add include as follow:
    -	../include
    -	../../groupsock/include
    -	../../UsageEnvironment/include
-	Add MediaServer (mediaServer)
  -	Add include as follow:
    -	../../liveMedia/include
    -	../../BasicUsageEnvironment/include
    -	../../groupsock/include
    -	../../UsageEnvironment/include
  -	Include libraries as follow:
    -	BasicUsageEnvironment.lib
    -	groupsock.lib
    -	liveMedia.lib
    -	UsageEnvironment.lib
    -	ws2_32.lib

