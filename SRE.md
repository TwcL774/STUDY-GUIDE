# SRE

- A Site Reliability Engineer (SRE) is a role that combines aspects of software engineering and systems administration to ensure the reliability, availability, and performance of an organization's systems and services.

- SREs are responsible for designing, building, and maintaining systems and services that are highly available, scalable, and performant. This includes tasks such as monitoring and responding to system issues, implementing automation to improve reliability and efficiency, and working with developers to design and implement new features and services.

- SREs work closely with software engineers and other technical teams to understand the requirements and constraints of the systems and services they are responsible for. They use this knowledge to identify and prioritize actions that will improve the reliability and performance of these systems.

- Some of the specific tasks and responsibilities that an SRE might have include:

  - Monitoring and alerting: Setting up and maintaining monitoring systems to identify and alert on potential issues or failures in the system.
  - Incident response: Responding to and resolving issues or outages as they arise. This may involve working with other teams to identify the root cause of the problem and implement a resolution.
  - Performance optimization: Identifying and addressing performance bottlenecks or issues in the system.
  - Capacity planning: Ensuring that the system has sufficient capacity to meet the needs of the organization.
  - Automation: Implementing automation to improve reliability, efficiency, and scalability of the system.
  - Tooling and infrastructure development: Building and maintaining tools and infrastructure that support the operation and maintenance of the system.

- SREs typically have a strong background in software engineering and systems administration, and they are skilled in programming, automation, and system design. They are also often familiar with agile development methodologies and are adept at working in a fast-paced, dynamic environment.

## SLA

- A Service Level Agreement (SLA) is a document that outlines the terms and conditions of a service provided by one party (the service provider) to another party (the customer). It specifies the level of service that the customer can expect from the service provider, including the availability, performance, and reliability of the service.

- An SLA may include details such as the specific services or functions that are included in the agreement, the levels of service that are promised (e.g. uptime, response times, etc.), the terms under which the service may be terminated or suspended, and any penalties or credits that may be applied in the event that the service provider fails to meet the agreed-upon terms.

- SLAs are commonly used in the context of IT services and are often used to establish expectations and accountability between a service provider and a customer. For example, a company may have an SLA with a cloud provider to ensure that their data and applications are available and accessible at all times.

- An SLA is not a one-size-fits-all document and is typically customized to meet the specific needs and requirements of the service provider and customer. It is important for both parties to carefully review and understand the terms of an SLA before agreeing to it, as it sets the expectations and terms of the service relationship.

## SLO

- A Service Level Objective (SLO) is a measurable target or goal that defines the level of service that a service provider aims to deliver to its customers. It is typically defined in terms of performance metrics such as availability, response time, or error rate, and it is used to establish the expectations and goals for the service being provided.

- SLOs are often used in conjunction with Service Level Agreements (SLAs), which are contracts that outline the terms and conditions of a service provided by one party (the service provider) to another party (the customer). SLOs are typically defined in the SLA and are used to measure and evaluate the performance of the service against the agreed-upon terms.

- For example, an SLO for a cloud storage service might specify that the service should be available 99.9% of the time and that data should be delivered within 100 milliseconds of a request. These SLOs would be used to measure the performance of the service and to determine whether the service provider is meeting the agreed-upon terms.

- In order to effectively measure and monitor SLOs, it is important to define clear and specific targets and to collect and analyze data on the relevant performance metrics. This allows service providers to track their progress and make any necessary adjustments to ensure that they are meeting the defined SLOs.

## SLI

- A Service Level Indicator (SLI) is a metric that is used to measure and monitor the performance of a service. It is a quantifiable measure of the quality or reliability of a service, and it is often used to track the service against Service Level Objectives (SLOs) or Service Level Agreements (SLAs).

- SLIs are typically defined in terms of performance metrics such as availability, response time, or error rate. For example, an SLI for a web application might be the percentage of requests that are successfully served within a certain time period, or the average time it takes for the application to respond to a request.

- SLIs are used to track the performance of a service over time and to identify any issues or trends that may impact the quality or reliability of the service. They can also be used to evaluate the effectiveness of changes or improvements made to the service.

- In order to effectively use SLIs, it is important to define clear and specific metrics that are relevant to the service being provided and to collect and analyze data on these metrics regularly. This allows service providers to track the performance of their service and to make any necessary adjustments to ensure that they are meeting their SLOs or SLAs.

## Error Budget

- An error budget is a tool that is used to manage the trade-off between reliability and innovation in software and IT systems. It is a set of guidelines and policies that dictate how much downtime or error rate is acceptable for a given service or system, and it provides a framework for making decisions about when and how to deploy new features or changes to the system.

- An error budget is typically expressed as a percentage of allowable downtime or error rate over a given period of time, such as a month or a quarter. For example, an error budget might specify that a service is allowed to have no more than 1% downtime per month, or that it is allowed to have no more than 0.1% error rate per quarter.

- The error budget serves as a way to balance the need for reliability with the desire to continuously improve and innovate. By setting limits on the amount of acceptable downtime or error rate, the error budget allows organizations to make informed decisions about when and how to roll out new features or changes to their systems, while still maintaining a certain level of reliability.

- Error budgets can be particularly useful for organizations that rely on highly available and scalable systems, such as cloud providers or e-commerce companies. By setting clear guidelines and expectations for downtime and error rates, error budgets can help organizations to manage their systems effectively and make informed decisions about when to deploy changes.

## Toil

- Toil is a term used to describe work that is repetitive, tedious, or lacks meaningful value. It is often used in the context of software engineering and IT operations to refer to tasks that are necessary but that do not contribute directly to the core goals or objectives of the organization.

Examples of toil in the context of software engineering and IT operations might include tasks such as manually performing routine maintenance on systems, fixing minor bugs, or responding to low-impact issues. Toil is often contrasted with more value-added work, such as developing new features or working on projects that have a direct impact on the business.

Toil can be a significant source of burnout and frustration for engineers and IT professionals, as it can be tedious and may not feel like meaningful or impactful work. It is important for organizations to identify and minimize toil where possible, in order to allow their teams to focus on more valuable and meaningful work. This may involve automating routine tasks, establishing clear processes and procedures, or outsourcing certain tasks to third-party providers.

## Incident Management

- The goal of incident management is to minimize the impact of an incident on the system and its users, and to restore normal operation as quickly as possible. This typically involves the following steps:

  - **Detection**: The incident must be detected as quickly as possible, either through automated monitoring or through manual reports from users or other team members.

  - **Triage**: Once an incident has been detected, it must be triaged to determine the severity of the incident and the appropriate response.

  - **Response**: The incident response team should take immediate action to mitigate the impact of the incident and to begin the process of restoring normal operation.

  - **Resolution**: Once the incident has been mitigated, the incident response team should work to identify and fix the root cause of the incident, to prevent it from happening again in the future.

  - **Communication**: Throughout the incident management process, it is important to keep all relevant parties informed about the status of the incident and the actions being taken to resolve it.

- Effective incident management requires a well-defined process and the appropriate tools and resources. It also requires a team of skilled and experienced professionals who are able to respond quickly and effectively to any unexpected events.

  1. Maintain a clear line of command

  2. Designate clearly defined roles

  3. Keep records of your work (debugging and mitigation actions)

  4. Declare incidents sooner rather than later

- Adding on to this, Google, in developing its SRE practices, draws inspiration from the Incident Command System designed by firefighters in 1968. In their system, there are three "C"s that help maintain focus and efficiency which Google uses to supplement their Incident Management guiding principles:

  - Coordinate

  - Communicate

  - Control

- As stated in the Google SRE handbook: "When something goes wrong with incident response, the culprit is likely in one of these areas. Mastering the 3Cs is essential for effective incident response."

## Leadership Roles

### Incident Commander

- a leadership role that is responsible for overall coordination of the incident response effort. The incident commander is responsible for setting the strategy for responding to an incident, allocating resources as needed, and making decisions about the direction of the response. They are often the primary point of contact for other teams and stakeholders during an incident, and is responsible for keeping them informed about the status of the incident and the actions being taken to resolve it.

- Some of the key responsibilities of an incident commander may include:

  - Assessing the severity and impact of the incident

  - Setting the overall strategy for responding to the incident

  - Allocating resources as needed, including technical expertise and support staff

  - Making decisions about the direction of the response effort

  - Coordinating with other teams and stakeholders to ensure that the incident is being properly managed

  - Providing updates and status reports to relevant parties

  - Working with the technical lead to identify the root cause of the incident and to implement a resolution

  - Coordinating with the communication lead to manage internal and external communication about the incident

### Technical Lead

- a leadership role that is responsible for overseeing the technical aspects of the incident response. This includes identifying the root cause of the incident and working to resolve it, as well as coordinating with other technical experts as needed to gather additional information or to implement solutions.

- Some of the key responsibilities of a technical lead may include:

  - Assessing the technical impact of the incident

  - Gathering and analyzing information about the incident to identify the root cause

  - Working with the incident commander and other technical experts to develop a plan to resolve the incident

  - Implementing solutions to resolve the incident

  - Coordinating with other teams, such as engineering and operations, to gather additional expertise or support as needed

  - Providing updates and status reports to the incident commander and other relevant parties

  - Ensuring that the incident is properly documented and that lessons learned are captured

### Communication Lead

- a leadership role that is responsible for coordinating all internal and external communications related to the incident. This includes keeping relevant parties informed about the status of the incident and the actions being taken to resolve it, as well as managing any public-facing communication about the incident.

- ome of the key responsibilities of a communication lead may include:

  - Developing and implementing a communication plan for the incident

  - Coordinating with the incident commander and other incident response leaders to gather information about the incident

  - Providing regular updates and status reports to relevant parties, including internal teams, customers, and external stakeholders

  - Managing internal and external communication channels, such as email, Slack, and social media

  - Ensuring that all communication is consistent and accurate

  - Handling any media inquiries or public-facing communication about the incident

  - Providing support and guidance to other teams as needed to ensure effective communication during the incident

#### Support Lead

- a leadership role that is responsible for coordinating support efforts for affected users and customers. This may include providing guidance and assistance to users, as well as coordinating with other teams to ensure that support requests are being addressed in a timely manner.

- Some of the key responsibilities of a support lead may include:

  - Coordinating the support efforts of various teams, such as customer service and technical support

  - Providing guidance and assistance to users and customers who are experiencing issues related to the incident

  - Gathering and analyzing information about user and customer needs and concerns related to the incident

  - Coordinating with other incident response leaders to ensure that support efforts are aligned with the overall response effort

  - Providing regular updates and status reports to relevant parties

  - Ensuring that support requests are being addressed in a timely and effective manner

  - Identifying and implementing strategies to improve the support experience for users and customers during and after the incident

## Incident Management: Postmortem

- An incident management postmortem is a review of an incident that occurred in a system, with the goal of identifying lessons learned and opportunities for improvement. The purpose of a postmortem is to understand what happened during the incident, why it happened, and what can be done to prevent similar incidents from occurring in the future. A postmortem should be conducted as soon after the incident as possible, while the details are still fresh in the minds of those involved. It is typically led by the incident commander or another senior leader, and may involve participation from a wide range of team members, including technical experts, support staff, and other relevant parties.

- A postmortem typically includes:

  - a detailed analysis of the incident, including the root cause

  - impact on the system and its users

  - the steps taken to resolve the incident

  - include recommendations for improving processes, tools, and procedures to reduce the likelihood of similar incidents occurring in the future.

- The results of the postmortem should be shared with all relevant parties, including management, technical teams, and other stakeholders. It is important to follow up on the recommendations and action items identified in the postmortem to ensure that any necessary improvements are implemented.

- A postmortem should be written for any significant incident that occurs in a system, regardless of whether it resulted in an outage or not. The goal of a postmortem is to understand what happened during the incident, why it happened, and what can be done to prevent similar incidents from occurring in the future.

- Some specific situations where a postmortem may be appropriate include:

  - Outages or other disruptions to service

  - Security breaches or other serious incidents

  - Incidents that caused significant impact to users or customers

  - Incidents that required significant effort to resolve

  - Incidents that exposed weaknesses or vulnerabilities in the system

- It is important to conduct a postmortem as soon after the incident as possible, while the details are still fresh in the minds of those involved. This will help to ensure that the root cause of the incident is accurately identified and that any necessary improvements can be implemented as quickly as possible.

## Postmortem: Blameless Culture

- A blameless postmortem is a review of an incident that is conducted in a way that does not place blame on any specific individuals or teams. The goal of a blameless postmortem is to identify the root cause of the incident and to identify opportunities for improvement, rather than to assign fault or responsibility. It typically involves a detailed analysis of the incident, including the events leading up to the incident, the impact on the system and its users, and the steps taken to resolve the incident. It may also include recommendations for improving processes, tools, and procedures to reduce the likelihood of similar incidents occurring in the future. One of the key benefits of a blameless postmortem is that it promotes a culture of continuous improvement, rather than one of blame and punishment. By focusing on the root causes of an incident and on identifying opportunities for improvement, organizations are better able to learn from their mistakes and to prevent similar incidents from occurring in the future.

## Tools

### [Grafana](https://grafana.com/grafana/)

- Grafana is an open-source data visualization and monitoring platform. It is often used to visualize and monitor time-series data, such as that collected by application and infrastructure monitoring tools. Grafana allows users to create custom dashboard panels that can display a variety of different types of data, including graphs, tables, and alerts. One of the key features of Grafana is its ability to connect to a wide range of data sources, including popular tools such as Prometheus, InfluxDB, and Elasticsearch. This allows users to bring data from multiple sources together into a single dashboard, making it easier to visualize and understand the relationships between different data sets. Grafana also includes a number of advanced features, such as the ability to create alerts based on data thresholds, and to annotate dashboard panels with comments and tags. It also includes a number of plugins that can be used to extend its functionality and add additional features.

### [Prometheus](https://prometheus.io/docs/introduction/overview/)

- Prometheus is an open-source monitoring and alerting system. It is designed to monitor and collect metrics from various systems, such as applications, servers, and storage systems, and to provide alerts based on defined thresholds or other rules.

- Prometheus includes a number of features that make it well-suited for use in dynamic, distributed systems:

  - Time-series data model: Prometheus stores all metrics as time-series data, making it easy to track and analyze changes in metric values over time.

  - Service discovery: Prometheus can automatically discover and monitor new targets that are added to the system, making it easy to scale monitoring as your system grows.

  - Alerting: Prometheus includes a powerful alerting system that can send notifications based on defined rules or thresholds.

  - Query language: Prometheus includes a flexible query language that allows users to slice and dice data in various ways, making it easy to extract the specific data points that you are interested in.

  - Exporters: Prometheus supports a wide range of exporters, which are libraries that can extract metrics from other systems and make them available to Prometheus for monitoring and alerting.

### Micrometer

- Micrometer is a Java library that provides a simple and consistent application programming interface (API) for instrumenting applications with metrics. It is designed to be used in a variety of environments, including Java SE, Java EE, and other runtimes, and to work with a variety of metrics backends. Micrometer provides a set of interfaces and classes that can be used to instrument application code with metrics, such as counters, gauges, and histograms. It also includes support for tags, which can be used to label metrics with additional context, such as the environment in which the code is running or the version of the application. One of the key benefits of Micrometer is its compatibility with a wide range of metrics backends, including popular tools such as Prometheus, InfluxDB, and Datadog. This allows developers to instrument their code with Micrometer and then choose the backend that best fits their needs, without having to modify their code.

### [Promtail](https://grafana.com/docs/loki/latest/clients/promtail/)

- Promtail (short for Prometheus Tail) is a logging agent that is part of the Loki project. It is designed to scrape log files from a variety of sources, such as application servers and containers, and to send the data to a Loki server for storage and analysis. Promtail is designed to be lightweight and easy to deploy, and can be run as a standalone binary or as a container. It supports a variety of input sources, including local files, Docker containers, and Kubernetes pods, and can extract metadata such as labels and pod names from the environment in which it is running.

- Promtail includes a number of features that make it well-suited for use in dynamic, distributed environments, such as:

  - Service discovery: Promtail can automatically discover new log sources as they become available, making it easy to scale logging as your system grows.

  - Label extraction: Promtail can extract metadata from the environment in which it is running, such as labels and pod names, and include it as part of the log data that it sends to the Loki server.

  - Query language: Promtail integrates with Loki's powerful query language, which allows users to slice and dice log data in various ways, making it easy to extract the specific data points that you are interested in.

### [Loki](https://grafana.com/oss/loki/)

- Loki is an open-source logging platform that is part of the Grafana Cloud offering. It is designed to be used in dynamic, distributed environments, such as cloud native applications, and to provide a scalable, efficient, and flexible logging solution.

- Loki consists of a number of components that work together to provide a complete logging solution:

  - Log scraper: Loki includes a log scraper, called Promtail, that is designed to scrape log files from a variety of sources, such as application servers and containers, and to send the data to the Loki server for storage and analysis.

  - Server: The Loki server is responsible for storing and indexing log data, and for providing a query interface for accessing and analyzing the data.

  - Query language: Loki includes a powerful query language that allows users to slice and dice log data in various ways, making it easy to extract the specific data points that you are interested in.

  - Grafana integration: Loki integrates with Grafana, which provides a rich set of visualization and analysis tools for exploring log data.
