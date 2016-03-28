This is an example to allow cross origin supported requests using @CrossOrigin support.

for testing we can run the application using mvn spring-boot:run for service, and client we can run using mvn spring-boot:run -Dserver.port=9000.

if a request comes from 9000 port then only service application can send the response, which can be configured in @CrossOrigin origins attribute. This can be done at class level,method level and globally by extending WebMvcConfigurerAdapter and @Overriding addCorsMappings method.
