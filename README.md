# Application Performance Monitoring with Elastic APM

# Elastic APM

Elastic APM (Application Performance Monitoring) helps you monitor software services and applications in real-time. It consists of four main components:

1. **Elasticsearch**: Stores and indexes the performance data.
2. **APM Agents**: Libraries that collect performance data from your applications.
3. **APM Server**: Receives data from APM agents and forwards it to Elasticsearch.
4. **Kibana APM UI**: Visualizes the performance data stored in Elasticsearch.

## Links

- [Elastic APM Overview](https://www.elastic.co/apm): Official Elastic APM page.
- [APM Server Reference](https://www.elastic.co/guide/en/apm/server/current/index.html): Documentation for APM Server.
- [Elastic APM JavaScript Agent](https://www.elastic.co/guide/en/apm/agent/rum-js/current/index.html): Documentation for the JavaScript APM agent.
- [Elastic APM Java Agent](https://www.elastic.co/guide/en/apm/agent/java/current/setup-javaagent.html): Documentation for the Java APM agent.

## Quickstart
## Configuration
### Set Permissions for APM Server Configuration File

```sh
icacls "C:\path\to\apm-server.yml" /inheritance:r /grant:r "Users:R" /grant:r "Administrators:F"
 ```

### Start APM Stack

To start the APM stack using Docker Compose, run the following command:

```sh
docker-compose -p apm up -d
 ```