Comandos

Arrancar jar
``` 
mvn run 
```

Web
````
http://localhost:8888/actuator/

"_links":{
    "self":{
        "href":"http://localhost:8888/actuator","templated":true
    },
    "health":{
        "href":"http://localhost:8888/actuator/health","templated":true
    },
    "health-component-instance":{
        "href":"http://localhost:8888/actuator/health/{component}/{instance}","templated":true
    },
    "health-component":{
        "href":"http://localhost:8888/actuator/health/{component}","templated":true
    },
    "info":{
        "href":"http://localhost:8888/actuator/info","templated":false
    }
  }
}
````

Web
```
http://localhost:8888/actuator/health

{"status":"UP"}
```

Web
```
http://localhost:8888/application/default

{"name":"application" , profiles:["default"], "label":null, "version":"...", "state":null, "propertySources":[{"name":"https://github.com/vicboma1/Arquitectura-SpringCloudConfig", "source":{"application.version":"1.0.0.0-SNAPSHOT",
"application.api.version":"api/v1/"}}]}
```