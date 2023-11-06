# promptail loki and grafana setup for Windows without docker

## 1. Download and setup promtail and loki

1. Go to [Github](https://github.com/grafana/loki/releases)
2. Expend Assets
3. Download loki-windows-amd64.exe.zip,promtail-windows-amd64.exe.zip
4. Extract loki-windows-amd64.exe.zip file into a folder somedire/loki
5. Create a loki config file config.yaml, make sure path are valid directories for widows
6. Extract promtail-windows-amd64.exe.zip file into a folder somedire/promtai
7. Create a promtail config file config.yaml, make sure path are valid directories for widowsl
8. use commands as
    
``` powershell
    cd somedir/loki
    loki-windows-amd64.exe --config.file config.yaml
    cd somedir/promtail
    promtail-windows-amd64.exe --config.file config.yaml
```

9. Verify loki endpoints http://localhost:3100/ready and http://localhost:3100/metrics

## Download and setup grafana

1. Go to [Github](https://github.com/grafana/grafana/releases)
2. Select the release version and click on download page like https://grafana.com/grafana/download/10.1.5
3. Download binaries
4. Unzip binaries to the folder somedir/grafana
5. Run following command

```powershell
    cd somedire/grafana/grafan-versionnumber/bin
    grafana-server.exe
```

6. <span style="color:red">Note grafana doesn't support internet explorer</span>

