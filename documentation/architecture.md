# Reticle


## Architecture highlights

### Real time event processing
Each microservice can produce events which will be queued and processed in (almost) real time by another microservice.


## Microservices

### router
HTTPS/2 endpoint that maps and load balances requests to their target microservice. Performs SSL offloading and certificate management. Should support Proxy Protocol and SNI.

### api
Validates authentication tokens and maps requests to microservices. Can also join or translate responses from multiple services to implement complex operations.

### core
Manages common data structures.

### cms (cds)
Headless content management and delivery system.

### renderer
Produces optimized HTML pages.

### assembler
Produces optimized javascript and css resources.

### event-processor
Processes events from the message queue and 

### shield

### ux360




## Data stores

### Couchbase
NoSQL data store. Each microservice stores its data in a vBucket.

### Etcd
Service discovery. Maybe can be used for cluster-wide configuration.

### RabbitMQ



## Core technologies

* Runtime: Node.js
* Languages: Typescript
* Containerization: Docker
* NoSQL Databases: Couchbase
* Queue system: RabbitMQ
* Frontend: Angular
* Templating: Handlebars, marko.js, riot
* Flex

### Inspiration

* Web designers: froont.com, webflow.com, wix.com, squarespace.com
* Content as a service: contentful.com, prismic.io, cloudcms.com, buttercms.com

## Templating and layouts

## Page rendering