# Microservice framework Roadmap

## v1.x
  - review code and fix bugs
  - minor improvements that does not affect backward compatibility with configuration and initialization 
  - expand tests coverage
  - release examples and improve documentation
  - implement autotesting
  - make stable releases for libraries and microservices
  
## v2.x
  - replace dotenv configurations with   JSON based config file (no more storing config data in process.env)
  - replace debug with custom log class with an ability to extend it by plugins (save logs to file, send by UDP/TCP to syslog server or any other plugins)
  - move microservice settings object to json config file (with an ability to set handlers function name)
  - integrate @microservice-framework/microservice-router-register to @microservice-framework/microservice.
    so service can register itself based on config file, instead of custom code in instance js file.
  - make sure that communication between microservices v1 and v2 are possible without any code changes to microservices v1 (backward compatibility)
  - implement `mfw create` to simplify process of developing new microservice.
  - implement admin page to microservice-router:admin service.It should display APM (Api performance monitor), ability to choose request distribution algorithm, ability to use Blue&green methodology.
  - implement scale microservice to automize horizontal scale functionality
