# Route53

Route53 on AWS provides DNS(resolves domain name to IP address) as a service.

As IP addresses can be statis or dynamic, incase they are dynamic the IP address will change for the resource and its difficult for user to use IP address hence we have domain names mapped to the IP address and this mapping is done by DNS.

There are 2 main parts to configure DNS - (1) Domain Registration(purchasing the domain name, example GoDaddy), (2)Hosting(hosting the records, example- Hostinger)
(1) Either we can purchase/register the domain from route53 or external sites.
(2) In Hosted zones we have to create the DNS records

Route53 also supports "Health checks", Route53 can perform health checks on the webserver, for example - if our application is hosted on 2 different Availability zones/ or 2 different web servers, so Route53 can simultaneously check the health of these servers, every 1min/5min it sends the request to the webservers and see's if this webserver is active or not, so based on the availability of these servers Route53 can return the IP of that server to the user.

Docs for Route53 - https://docs.aws.amazon.com/route53/
