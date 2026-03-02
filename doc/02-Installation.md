# Installation

## From source

1. Clone a Icinga Web Performance Data Graphs Backend repository into `/usr/share/icingaweb2/modules/perfdatagraphsprometheus/`

2. Enable the module using the `Configuration → Modules` menu or the `icingacli`

3. Configure the Prometheus URL, organization, bucket and authentication using the `Configuration → Modules` menu

# Configuration

`config.ini` - section `prometheus`

| Option                      | Description                                                                                              | Default value            |
|-----------------------------|----------------------------------------------------------------------------------------------------------|--------------------------|
| api_url              | The URL for Prometheus including the scheme                                                                | `http://localhost:9090`  |
| api_timeout          | HTTP timeout for the API in seconds. Should be higher than 0                                             | `10` (seconds)           |
| api_max_data_points  | The maximum numbers of datapoints each series returns. Aggregation can be disabled by setting this to 0. | `10000`                  |
| api_tls_insecure     | Skip the TLS verification                                                                                | `false` (unchecked)      |
