---
layout: default
---
# Quickstart

Start a docker container for confrm server:

```bash
docker run -d -p 8000:80 --name confrm_server -v /var/confrm:/confrm confrm/confrm:latest
```

Navigate to the user interface (i.e. http://127.0.0.1:8000).

Add confrm to your ESP32 project (Arduino IDE):

```cpp
#include <confrm.h>
Confrm *confrm;
```

And in the setup() function:

```cpp
confrm = new Confrm(...);
```


