# Topics
## Project Generator

- [Spring Boot](http://projects.spring.io/spring-boot/#quick-start)
- [Spring Initializr](https://start.spring.io/)

## Web Services
### Tutorial
- [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)
- [Building a RESTful Web Service with Spring Boot Actuator](https://spring.io/guides/gs/actuator-service/)

## HandsON
* **Controller:** _new file with the implemented methods._
````	
  @Service
	public class EventStatusController
````	
* **Configuration (config):** _new file pointing to the controller file._
````	
  @Configuration
	public class EventStatusConfig {

	    @Bean
	    EventStatusController eventStatusController(){
	        return new EventStatusController();
	    }
	}
````
* **ContextListener:** _add a reference to the configuration file._
````
  classes.add(EventStatusConfig.class);
````

* **Resource:** _add a reference to the controller._
````
  @Autowired
	EventStatusController eventStatusController;

[...]

    @POST
    @Path("/statusEvent")
    public Response eventStatusController(StatusRequest statusRequest){
        return eventStatusController.checkAndDelete(statusRequest);
    }	
````

* **New Files:**
  * EventStatusController
  * EventStatusConfig
