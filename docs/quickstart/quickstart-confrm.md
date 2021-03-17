# Basic Confrm Server

## Docker

The easiest way to deploy confrm is to use Docker, it is pre-packaged and works with most platforms. A server can be launched using:

```
docker run -d --restart=unless-stopped -p 8000:80 --name confrm confrm/confrm:latest
```

By default the data will be stored inside the container, it can be exposed using by running the container using:

```
docker run -d --restart=always -v /path/to/data:/confrm -p 8000:80 --name confrm confrm/confrm:latest
```

The contents of /path/to/data can then be easily backed up.

## Native Python

The git repository can be installed using pip and run as follows:

```
pip install --user git+https://github.com/confrm/confrm.git
```

You will need to set up a configuration file in the following form:

``` toml
[basic]
port = 80
host = "0.0.0.0"

[storage]
data_dir = "/path/to/store"
```

After creating the config file, and specifying a data directory the server is started using:

``` bash
confrm_srv --config=/path/to/config
```
