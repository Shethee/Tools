Elastic Slack is a tool used for log analysis and investigations. It is not a traditional SIEM. Many SOC use it for Data searching and visualization capability.
1. Components of ELK and their use in SOC
2. Different features of ELK
3. Search and Filter data in ELK
4. VPN logs to identify anomalies

### Elastic Search
First componet, is a full text search and analytics engine for JSON formatted documents. It stores analyzes and correlates data and supports a RESTful API for interacting with it
### Logstash
It is a data processing engine that takes data from different sources, filters and normalize it and then sends it to the destination which could be kibana or a llistening port. A logstash configuration files is divided into three parts.
1. The input part is where the user defines the source from which the data is being ingested.
2. The filter [art is where the user specifies the filter options to normalize the log instead above.
3. The output part is where the user wants the filtered data to be sent. It can be listening port, kibana interface, Elasticsearch database or file.

### Beats
It is a host based agent known as data shippers that ship/transfer data from the endpoints to elasticsearch. Each beat is a single purpose agent that sends specific data to elasticsearch.

### Kibana
Kibana is a web based data visualization tool that works with Elasticsearch to analyze, investigate and visualize data streams in real time. It allows users to create multiple visualizations and dashboards for better visibility.

1. Beats collect data from multiple agents. For example, Winlogbeat collects Windows event logs, and Packetbeat collects network traffic flows.
2. Logstash collects data from beats, ports, or files, parses/normalizes it into field value pairs, and stores them into Elasticsearch.
3. Elasticsearch acts as a database used to search and analyze data.
4. Kibana is responsible for displaying and visualizing the data stored in Elasticsearch. The data stored in Elasticsearch can easily be shaped into different visualizations, time charts, infographics, etc., using Kibana.
