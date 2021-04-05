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

Visitar via web JSON con el fichero application.properties de nuestro repo centralizado
```
http://localhost:8888/application/default
```