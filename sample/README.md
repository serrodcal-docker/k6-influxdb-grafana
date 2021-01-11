# Sample

1. Start InfluxDB and Grafa using one of the options provided, docker-compose or k8s

2. Open Grafana in a browser: [http://localhost:3000/](http://localhost:3000/)

3. Run the sample with:

    ```sh
    $ docker run --rm -it -p 8080:8080 serrodcal/doctor:1.0.0-native 
    ```

4. Run the test scenario with:

    ```sh
    $ k6 run --out influxdb=http://localhost:8086/k6 script.js
    ```