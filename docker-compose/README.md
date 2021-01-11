# Docker Compose

1. Up InfluxDB and Grafana:

    ```sh
    $ docker-compose up -d influxdb grafana
    ```

2. Open Grafana in a browser: [http://localhost:3000/](http://localhost:3000/)

3. Run the script as follow:

    ```sh
    $ k6 run --out influxdb=http://localhost:8086/k6 script.js 
    ```

Check out the [sample](sample).

Finally, clean up with:

```sh
$ docker-compose down
```

