# curator

### curator.md

1. install curator

    `pip3 install curator`

2. edit config
    -  curator.sh 
    ```
    /<path>/<to>/.local/bin/curator
    ex. /home/<username>/.local/bin/curator
    ```
    -  curator.yml
    ```
    http_auth: "<user>:<password>"
    logfile: <path>/<to>/log/curator.log
    ```

3. set crontab
    - 3.1 edit
    ```
    crontab -e
    
    0 3 * * * /bin/bash /var/service-curator-elk/curator.sh
    ```
    - 3.2 confirm
        
    ```
    crontab -l
    ```