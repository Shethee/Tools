SPLUNK is a one of the leading SIEM solution in the market. It allows users to collect, analyze and correlate newtwork and machine logs in real time. \
. Ingestion in splunk(need to study)
=> splunk has three main components which are Forwarder, Indexer and Search head. these helps to search and analyze data. \
### splunk forwarder
. it is the main task to collect data and sent it to the splunk instance. 
. it does not affect the endpoints performance as it takes a few resources to process.
=> some of the key data sources are:
1. Web server generating web traffic
2. windows machine generating windows event logs, powershell and sysmon data
3. linux host generating host-centric logs
4. database generating DB connection requests, response and errors.
=> the forwarder collects the data from the log sources and sends it to the splunk indexer.
### Splunk indexer
. Splunk indexer plays the main role in processing the data it receives from forwarders. It passes and normalize
the data info field value pairs and stores the results as events, making the processed data easy to search and analyze.
### Search head
. Splunk search head is the place within the search and reporting app where users can search the indexed logs. The searches are done using the SPl(Search Processing Language).
a powerful query language for searching indexed data. when the user performs a search, the request is sent to the indexer and the relevant events are returned as field value pairs.



