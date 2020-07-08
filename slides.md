---
title: Service Mesh
---

<!-- .slide: class="master01" -->

# Service Mesh

---

<!-- .slide: class="text-left" -->
### Service Mesh Definition

A service mesh is a decentralized application networking infrastructure among your services that provides resiliency, security, observability, and routing control. 

---

<!-- .slide: class="text-left" -->
### Service Mesh & API Gateway overlap

<div class="container">
<div class="col">

* Telemetry collection
* Distributed tracing
* Service discovery
* Load balancing
* TLS term-/origination
* JWT validation

</div>
<div class="col">

* Request routing
* Traffic splitting
* Canary releasing
* Traffic shadowing
* Rate limiting

</div>
</div>

---

<!-- .slide: class="text-left" -->
### Service Mesh & API Gateway Differences

 API Gateway:
  * Is focused on business functionality
  * Handles external client-to-service communication
  * Abstracts and decouples service implementations

---

<!-- .slide: class="text-left" -->
### Service Mesh & API Gateway Differences

Service Mesh:
  * Is focused on network
  * Handles internal service-to-service communication
  * Provides details about service implementations

---

<!-- .slide: class="text-left" -->
### Unique API Gateway capabilities

* Boundary decoupling
* Tight control over data are allowed in and out
* Bridging security trust domains

---

<!-- .slide: class="text-left" -->
### API Gateway Boundary Decoupling

* Request / response transformation
* Application protocol transformation like REST/SOAP/XSLT
* Error / Rate limit custom responses
* Direct responses, e.g. blocked clients/requests
* Precise control over api/proxy pipelining
* API composition/grouping

---

<!-- .slide: class="text-left" -->
### Do I Need a Service Mesh?

You may need one if:
* You're using a microservices architecture
* And you’re deploying to a cloud platform
* And implement services with different languages/frameworks

---

<!-- .slide: class="text-left" -->
### Service Mesh Tradeoffs

* Increased resource usage
* Increased latency
* Increased operations complexity

---

<!-- .slide: class="text-left" -->
### Red Hat Service Mesh Components

| Component            | Version |
| -------------------- | ------- |
| Istio                | 1.4.8   |
| Jaeger               | 1.17.3  |
| Kiali                | 1.12.7  |
| 3scale Istio Adapter | 1.0.0   |

<small>References: <small>[1]</small></small>

[1]: https://docs.openshift.com/container-platform/4.4/service_mesh/servicemesh-release-notes.html#component-versions-included-in-red-hat-openshift-service-mesh-version-1-1-4

---

<!-- .slide: class="text-left" -->
### Red Hat Service Mesh OAuth/OIDC

Requires Istio Adapter:

* App Identity and Access Adapter <small>[1] [2]</small>
* API Gateway and adapter, e.g. 3scale adapter <small>[3]</small>

[1]: https://github.com/ibm-cloud-security/app-identity-and-access-adapter
[2]: https://istio.io/latest/blog/2019/app-identity-and-access-adapter/
[3]: https://docs.openshift.com/container-platform/4.4/service_mesh/threescale_adapter/threescale-adapter.html

---

<!-- .slide: class="text-left" -->
### What's Next

* https://blog.christianposta.com/microservices/do-i-need-an-api-gateway-if-i-have-a-service-mesh/
* https://medium.com/microservices-in-practice/service-mesh-vs-api-gateway-a6d814b9bf56
* https://medium.com/microservices-in-practice/service-mesh-for-microservices-2953109a3c9a
* https://leanpub.com/service-mesh-primer


