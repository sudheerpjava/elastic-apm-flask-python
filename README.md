# Elastic APM python configuration

## 1.Add below configuration on Flask app to integrate with elastic apm
```
service_url = <ELASTIC_SERVER_URL>
service_name = <APP_NAME>
```
#######################################################################
```
from elasticapm.contrib.flask import ElasticAPM
from elasticapm.handlers.logging import LoggingHandler
apm = ElasticAPM(app, server_url='http://localhost:8200', service_name='flask-app-1', logging=True)
```
 