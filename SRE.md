# SRE

* A Site Reliability Engineer (SRE) is a role that combines aspects of software engineering and systems administration to ensure the reliability, availability, and performance of an organization's systems and services.

* SREs are responsible for designing, building, and maintaining systems and services that are highly available, scalable, and performant. This includes tasks such as monitoring and responding to system issues, implementing automation to improve reliability and efficiency, and working with developers to design and implement new features and services.

* SREs work closely with software engineers and other technical teams to understand the requirements and constraints of the systems and services they are responsible for. They use this knowledge to identify and prioritize actions that will improve the reliability and performance of these systems.

* Some of the specific tasks and responsibilities that an SRE might have include:

    * Monitoring and alerting: Setting up and maintaining monitoring systems to identify and alert on potential issues or failures in the system.
    * Incident response: Responding to and resolving issues or outages as they arise. This may involve working with other teams to identify the root cause of the problem and implement a resolution.
    * Performance optimization: Identifying and addressing performance bottlenecks or issues in the system.
    * Capacity planning: Ensuring that the system has sufficient capacity to meet the needs of the organization.
    * Automation: Implementing automation to improve reliability, efficiency, and scalability of the system.
    * Tooling and infrastructure development: Building and maintaining tools and infrastructure that support the operation and maintenance of the system.

* SREs typically have a strong background in software engineering and systems administration, and they are skilled in programming, automation, and system design. They are also often familiar with agile development methodologies and are adept at working in a fast-paced, dynamic environment.

## SLA

* A Service Level Agreement (SLA) is a document that outlines the terms and conditions of a service provided by one party (the service provider) to another party (the customer). It specifies the level of service that the customer can expect from the service provider, including the availability, performance, and reliability of the service.

* An SLA may include details such as the specific services or functions that are included in the agreement, the levels of service that are promised (e.g. uptime, response times, etc.), the terms under which the service may be terminated or suspended, and any penalties or credits that may be applied in the event that the service provider fails to meet the agreed-upon terms.

* SLAs are commonly used in the context of IT services and are often used to establish expectations and accountability between a service provider and a customer. For example, a company may have an SLA with a cloud provider to ensure that their data and applications are available and accessible at all times.

* An SLA is not a one-size-fits-all document and is typically customized to meet the specific needs and requirements of the service provider and customer. It is important for both parties to carefully review and understand the terms of an SLA before agreeing to it, as it sets the expectations and terms of the service relationship.

## SLO

* A Service Level Objective (SLO) is a measurable target or goal that defines the level of service that a service provider aims to deliver to its customers. It is typically defined in terms of performance metrics such as availability, response time, or error rate, and it is used to establish the expectations and goals for the service being provided.

* SLOs are often used in conjunction with Service Level Agreements (SLAs), which are contracts that outline the terms and conditions of a service provided by one party (the service provider) to another party (the customer). SLOs are typically defined in the SLA and are used to measure and evaluate the performance of the service against the agreed-upon terms.

* For example, an SLO for a cloud storage service might specify that the service should be available 99.9% of the time and that data should be delivered within 100 milliseconds of a request. These SLOs would be used to measure the performance of the service and to determine whether the service provider is meeting the agreed-upon terms.

* In order to effectively measure and monitor SLOs, it is important to define clear and specific targets and to collect and analyze data on the relevant performance metrics. This allows service providers to track their progress and make any necessary adjustments to ensure that they are meeting the defined SLOs.

## SLI

* A Service Level Indicator (SLI) is a metric that is used to measure and monitor the performance of a service. It is a quantifiable measure of the quality or reliability of a service, and it is often used to track the service against Service Level Objectives (SLOs) or Service Level Agreements (SLAs).

* SLIs are typically defined in terms of performance metrics such as availability, response time, or error rate. For example, an SLI for a web application might be the percentage of requests that are successfully served within a certain time period, or the average time it takes for the application to respond to a request.

* SLIs are used to track the performance of a service over time and to identify any issues or trends that may impact the quality or reliability of the service. They can also be used to evaluate the effectiveness of changes or improvements made to the service.

* In order to effectively use SLIs, it is important to define clear and specific metrics that are relevant to the service being provided and to collect and analyze data on these metrics regularly. This allows service providers to track the performance of their service and to make any necessary adjustments to ensure that they are meeting their SLOs or SLAs.

## Error Budget

* An error budget is a tool that is used to manage the trade-off between reliability and innovation in software and IT systems. It is a set of guidelines and policies that dictate how much downtime or error rate is acceptable for a given service or system, and it provides a framework for making decisions about when and how to deploy new features or changes to the system.

* An error budget is typically expressed as a percentage of allowable downtime or error rate over a given period of time, such as a month or a quarter. For example, an error budget might specify that a service is allowed to have no more than 1% downtime per month, or that it is allowed to have no more than 0.1% error rate per quarter.

* The error budget serves as a way to balance the need for reliability with the desire to continuously improve and innovate. By setting limits on the amount of acceptable downtime or error rate, the error budget allows organizations to make informed decisions about when and how to roll out new features or changes to their systems, while still maintaining a certain level of reliability.

* Error budgets can be particularly useful for organizations that rely on highly available and scalable systems, such as cloud providers or e-commerce companies. By setting clear guidelines and expectations for downtime and error rates, error budgets can help organizations to manage their systems effectively and make informed decisions about when to deploy changes.

## Toil

* Toil is a term used to describe work that is repetitive, tedious, or lacks meaningful value. It is often used in the context of software engineering and IT operations to refer to tasks that are necessary but that do not contribute directly to the core goals or objectives of the organization.

Examples of toil in the context of software engineering and IT operations might include tasks such as manually performing routine maintenance on systems, fixing minor bugs, or responding to low-impact issues. Toil is often contrasted with more value-added work, such as developing new features or working on projects that have a direct impact on the business.

Toil can be a significant source of burnout and frustration for engineers and IT professionals, as it can be tedious and may not feel like meaningful or impactful work. It is important for organizations to identify and minimize toil where possible, in order to allow their teams to focus on more valuable and meaningful work. This may involve automating routine tasks, establishing clear processes and procedures, or outsourcing certain tasks to third-party providers.
