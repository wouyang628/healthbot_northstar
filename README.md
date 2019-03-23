# Self Healing on the WAN with Healthbot and Northstar Controller
Healthbot Northstar integration
1. Healthbot monitors link latency via Streaming Telemetry
 
2. When delay of a link goes above 200ms, Healthbot sends out a notification to a third party listener
 
3. After receiving the notification, the listener requests a Failure Analysis in Northstar controller via REST API 
 
4. If the Failure Analysis passes, it then requests a link maintenance event in Northstar
 
5. This triggers Northstar to automatically reroute the LSPs to avoid that link

Please refer to Wifi on how to set it up.
