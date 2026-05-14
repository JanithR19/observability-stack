FROM grafana/alloy:latest

# Copy the configuration file
COPY config.alloy /etc/alloy/config.alloy

# Expose the necessary ports
EXPOSE 4317 4318 12345

# Start Alloy with the configuration
CMD ["run", "--server.http.listen-addr=0.0.0.0:12345", "--stability.level=experimental", "/etc/alloy/config.alloy"]