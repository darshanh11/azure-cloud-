#  Azure Traffic Management

## Azure Load Balancer

### Explanation

Azure Load Balancer is a Layer 4 load-balancing service that distributes incoming network traffic across multiple backend resources such as Virtual Machines.

It improves application availability and scalability by distributing traffic between healthy backend instances.

### Steps to Create an Azure Load Balancer

1. Sign in to the **Azure Portal**.
2. Search for **Load Balancers**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Load Balancer name**.
7. Select the required **Region**.
8. Select the required **SKU**.
9. Select the required **Type**, such as Public or Internal.
10. Configure the **Frontend IP configuration**.
11. Configure the **Backend pool**.
12. Configure the required **Health probe**.
13. Configure the required **Load balancing rule**.
14. Review the configuration.
15. Select **Review + create**.
16. Select **Create**.

## screenshot
![Azure Load Balancer](../image01.png)
-->

---

## Azure Application Gateway

### Explanation

Azure Application Gateway is a Layer 7 web traffic load balancer. It can route HTTP and HTTPS traffic based on information such as URL paths and host names.

It also supports features such as SSL/TLS termination, autoscaling, and integration with Web Application Firewall.

### Steps to Create an Application Gateway

1. Sign in to the **Azure Portal**.
2. Search for **Application Gateways**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Application Gateway name**.
7. Select the required **Region**.
8. Select the required **Tier**.
9. Configure the **Virtual Network**.
10. Configure the required **Frontend IP configuration**.
11. Configure the **Backend pool**.
12. Configure the **Backend settings**.
13. Configure the required **Routing rule**.
14. Configure the **Listener**.
15. Configure the **Health probe** if required.
16. Review the configuration.
17. Select **Review + create**.
18. Select **Create**.


## screenshot
![Azure Application Gateway](../image02.png)
-->

---

## Web Application Firewall (WAF)

### Explanation

Web Application Firewall (WAF) helps protect web applications from common web-based attacks.

It can inspect HTTP and HTTPS requests and block or allow traffic according to configured security rules.

WAF can be integrated with services such as Azure Application Gateway and Azure Front Door.

### Steps to Configure WAF

1. Sign in to the **Azure Portal**.
2. Search for **Web Application Firewall policies**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **WAF policy name**.
7. Select the required **Region** if applicable.
8. Select the required **Policy mode**.
9. Configure the required **Managed rules**.
10. Configure custom rules if required.
11. Review the configuration.
12. Select **Review + create**.
13. Select **Create**.
14. Associate the WAF policy with the required supported resource.


## screenshot
![Azure Web Application Firewall](../image03.png)
-->

---

## Azure Traffic Manager

### Explanation

Azure Traffic Manager is a DNS-based traffic routing service. It directs users to the appropriate application endpoint based on a configured traffic-routing method.

Traffic Manager can use routing methods such as Priority, Weighted, Performance, Geographic, Multivalue, and Subnet.

### Steps to Create Azure Traffic Manager

1. Sign in to the **Azure Portal**.
2. Search for **Traffic Manager profiles**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Traffic Manager profile name**.
7. Select the required **Routing method**.
8. Configure the required endpoint.
9. Add the required application endpoints.
10. Configure endpoint monitoring.
11. Review the configuration.
12. Select **Create**.
13. Test the Traffic Manager profile.


## screenshot
![Azure Traffic Manager](../image04.png)
-->

---

## Azure Front Door

### Explanation

Azure Front Door is a global application delivery service that provides Layer 7 routing for web applications.

It can provide global traffic distribution, acceleration, TLS termination, health monitoring, caching, and integration with Web Application Firewall.

### Steps to Create Azure Front Door

1. Sign in to the **Azure Portal**.
2. Search for **Front Door and CDN profiles**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the **Front Door profile name**.
7. Select the required **Tier**.
8. Configure the **Endpoint**.
9. Configure the **Origin group**.
10. Add the required **Origin**.
11. Configure the required **Route**.
12. Configure health probes if required.
13. Configure WAF if required.
14. Review the configuration.
15. Select **Create**.

## screenshot
![Azure Front Door](../image05.png)
-->

---

## Content Delivery Network (CDN)

### Explanation

A Content Delivery Network (CDN) distributes cached content through geographically distributed edge locations.

CDN reduces latency by serving content from an edge location closer to the user instead of always retrieving it from the origin server.

Azure provides content delivery capabilities through its current Front Door-based offerings.

### Steps to Configure Content Delivery

1. Sign in to the **Azure Portal**.
2. Search for **Front Door and CDN profiles**.
3. Select **Create**.
4. Select the required **Subscription**.
5. Select or create a **Resource Group**.
6. Enter the required **Profile name**.
7. Select the required **Tier**.
8. Configure the required **Endpoint**.
9. Configure the **Origin**.
10. Configure the required **Route**.
11. Configure caching settings if required.
12. Review the configuration.
13. Select **Create**.
14. Test the endpoint.


## screenshot
![Azure CDN](../image06.png)
-->

---
