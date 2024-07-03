# YARP Authentication

There are a few sample requests you can send from the `gateway.http` file.
The gateway is configured to use token authentication, so you can easily test this. 

```
@BaseUrl =
@AccessToken =

### Login - pass `isVip=true` to add the respective claim

GET {{BaseUrl}}/login?isVip=true

### Proxy api/hello

GET {{BaseUrl}}/api/hello
Authorization: Bearer {{AccessToken}}

### Proxy api/hello-vip

GET {{BaseUrl}}/api/hello-vip
Authorization: Bearer {{AccessToken}}
```

**Whenever you're ready, there are 2 ways I can help you:**:

1. [**Pragmatic Clean Architecture:**](https://www.milanjovanovic.tech/pragmatic-clean-architecture?utm_source=dev.to&utm_medium=website&utm_campaign=cross-posting) Join 2,900+ students in this comprehensive course that will teach you the system I use to ship production-ready applications using Clean Architecture. Learn how to apply the best practices of modern software architecture.
 
2. [**Modular Monolith Architecture:**](https://www.milanjovanovic.tech/modular-monolith-architecture?utm_source=dev.to&utm_medium=website&utm_campaign=cross-posting) Join 750+ engineers in this in-depth course that will transform the way you build modern systems. You will learn the best practices for applying the Modular Monolith architecture in a real-world scenario.
