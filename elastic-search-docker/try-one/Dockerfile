FROM logstash:7.17.0

# Switch to root to create the directory
USER root

# Create the directory with the necessary permissions
RUN mkdir -p /opt/logstash-mongodb/ && chown -R logstash:logstash /opt/logstash-mongodb/

# Switch back to the logstash user
USER logstash

# Install the MongoDB input plugin
RUN logstash-plugin install logstash-input-mongodb
