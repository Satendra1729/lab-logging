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

## Evolution

### Setup Loki Promtail Grafana for local logs

    1. Done all works good
    2. For windows set __path__ to correct log path

### Push logs from remote windows machine

    1. Pending

### Add Promethus system metrics

    1. Pending

### Setup

    1. Replace TARGET_DIR value at per environment, it should be point to src folder.
    2. Run 
```bash 
        cd src
        docker-compose --env-file .env up -d --force-recreate
```

## References

   1. [Meet Grafana LOKI, a Log Aggregation System for EVERYTHING](https://www.youtube.com/watch?v=h_GGd7HfKQ8)