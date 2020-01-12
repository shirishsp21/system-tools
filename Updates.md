Following updates have been made in the fork:
-  i) Make check interval for node stats configurable using environment variable - NODE_STAT_CHECK_INTERVAL_SECS
-  ii) Added functionality to post the stat info to a monitoring agent when environment variable - 'MONITORING_AGENT_HOOK_ENABLED' is true.
   Data will be posted to monitoring agent listening at url specified in environment variable - 'MONITORING_AGENT_URL'
   Other environment variables for monitoring agent:

	- MONITORING_AGENT_AUTH_KEY - basic auth scheme encoded user:pass key.
	- MONITORING_AGENT_DATA_FORMAT - data format (eg 'system-tools-raw') type to inform the monitoring agent about what type of data is being posted.
	- MONITORING_NODE_ID - specifies which node or nodes the posted data is for.
