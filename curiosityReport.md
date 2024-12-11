# Load Balancers in AWS

## What are load balancers?

Load balancers equally distribute network traffic between resources. They work as a facilitator to make sure that all of the servers in a network are used.

## What are the benefits?

AWS load balancers provide four benefits: performance, scalability, availability, and security.

### Performance

Load balancers help to prevent servers from becoming overloaded by distributing traffic between multiple services. They route traffic to the optimal server which results in faster response times.

### Scalability

Load balancers are able to scale horizontally and can handle thousands of requests per second. By splitting traffic between multiple servers, load balancers prevent bottlenecks.

### Availability

Load balancers actively detect unhealthy servers and will direct traffic to the servers that are healthy. They provide a way to do server maintenance without downtime.

### Security

Load balancers provide another layer of security. You can monitor your traffic and run requests through firewalls.

## What are the different algorithms?

There are several algorithms that load balancers can take advantage of.

### Static load balancing uses the following algorithms:

- Round-robin method
- Weighted round-robin method
- IP hash method

### Dynamic load balancing uses the following algorithms:

- Least connection method
- Weighted least connection method
- Least response time method
- Resource-based method

## What are the costs?

- $0.0225 per Application Load Balancer-hour and $0.008 per LCU-hour
- $0.0225 per Network Load Balancer-hour and $0.006 per NLCU-hour
- $0.0125 per Gateway Load Balancer-hour per AZ and $0.004 per GLCU-hour
- $0.025 per Classic Load Balancer-hour and $0.008 per GB of data processed by a Classic Load Balancer

The cost for using a load balancer depends on your traffic, but you are looking at $15+ per month.

## Overall thoughts

Load balancers provide many benefits to applications, especially as they scale. They follow some of the principles that we learned in this class like adding redundancy and providing a way to run server maintenance without downtime. The cost for the benefits seems relatively low, but it may greatly increase if your application gets thousands of requests. They also provide another layer of security, an important step in DevSecOps. I plan on leveraging load balancers in feature work. 