# Logging

## Target Technology

    1. Docker
    2. Grafana
    3. Loki
    4. Promtail
    5. Loki Logging Driver

## Log Sources

    1. Local System
    2. Docker
    3. Syslog
    4. Remote System 
        4.1. Install Promtail to the target server
        4.2. Create Configuration to point it to the loki endpoint
        4.3. Start Promtail with above config and verify the log collection 

## References

    1. [Meet Grafana LOKI, a Log Aggregation System for EVERYTHING](https://www.youtube.com/watch?v=h_GGd7HfKQ8)