# pcwt

*Engineering robust, modular, and scalable B2B SaaS infrastructure.*

> ### engineering principles
>
> * **First-Principles Design**: *Lightweight, self-hosted, and robust microservices architecture* with minimal external bloat.
> * **Tenant Isolation**: Strict data separation per namespace backed by lazy schema initialization.
> * **Resilience**: Best-effort cross-service communications ensuring core operations never fail if secondary integrations experience downtime.



## the [lota](https://lota.tools) ecosystem

**lota** is our flagship multi-tenant B2B SaaS ecosystem designed for high-load operations, retail, HoReCa, and service-driven businesses. Built with a *modular microservices architecture*, it provides complete isolation per tenant workspace while maintaining *seamless cross-service integration*.

### core components
* **Hub**: Platform core for unified authentication, multi-tenant namespace management, RBAC, invites, and operator console.
* **Capital**: Financial and content engine for tariff plans, quota enforcement, subscription lifecycle, invoicing, and knowledge bases.
<details>
<summary><b>view ecosystem apps</b></summary>

<br/>

* <b>Atrace</b>: Attendance and payroll engine for shift patterns, geofenced check-ins, and route tracking.
* <b>Contacts</b>: Centralized CRM and loyalty database for customer records, custom dynamic fields, and bonus systems.
* <b>Menu / Orders</b>: Digital storefronts and order management with multi-branch catalogs, modifiers, and kitchen display boards.
* <b>Issues</b>: Dispatch and task management featuring customizable Kanban boards, SLA escalations, and real-time tracking.
* <b>Goods</b>: Inventory and POS system for multi-warehouse tracking, stock movements, and recipe-based ingredient auto-deduction.
* <b>Plans</b>: Scheduling and online booking for calendar management, staff availability, and client booking portals.
* <i>And etc, as we continue to develop and add new services to our ecosystem.</i>

</details>


## microservices architecture and templates

We enforce *strict templates* for our microservices and etc, ensuring absolute consistency across code structure, contracts, server implementation, and API gateways. Every service follows strict separation patterns, independent storage per namespace, and resilient best-effort cross-service communications.

### core architecture repositories & tooling
To maintain this strict consistency, our ecosystem is built upon *standard reference templates*, *shared libraries*, and *automation pipelines*:
* **[`.sample.proto`](https://github.com/pieceowater-dev/lotof.sample.proto)** — *Reference contract template repository defining standard gRPC and Protobuf schemas.*
* **[`.sample.svc`](https://github.com/pieceowater-dev/lotof.sample.svc)** — *Reference business logic server template implementing core domain workflows.*
* **[`.sample.gtw`](https://github.com/pieceowater-dev/lotof.sample.gtw)** — *Reference API gateway template acting as the single web entry point and routing layer.*
* **[`.lib.gossiper`](https://github.com/pieceowater-dev/lotof.lib.gossiper)** — *Core internal shared library utilized across our microservices ecosystem.*
* **[`.cloud.ci`](https://github.com/pieceowater-dev/lotof.cloud.ci)** — *Cloud CI/CD automation pipeline configurations and tooling for continuous delivery.*


<details>
<summary><b>technology stack</b></summary>

<br/>

* **Languages & Protocols**: Go, TypeScript, gRPC, GraphQL
* **Infrastructure & Deployment**: Docker, Kubernetes, Terraform, Ansible, AWS
* **Environments**: Linux, macOS

</details>


### links & resources
* *Explore our internal guidelines and architecture specs in the [Organization Wiki](https://github.com/pieceowater-dev/.github/wiki).*
