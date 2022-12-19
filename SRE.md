# SRE
    It is a discipline that combines software engineering and operations to ensure that software systems are scalable, reliable, and highly available. SRE teams focus on building and maintaining the infrastructure and processes needed to keep software systems running smoothly and efficiently. They are responsible for tasks such as monitoring systems for issues, responding to incidents, and implementing automation to improve reliability. SRE is a relatively new field that has grown in popularity in recent years as organizations have increasingly relied on complex, large-scale software systems to support their operations.

## SLO
    - Service Level Objectives (SLOs) are performance targets that are set for a service or system. They are typically defined in a service level agreement (SLA) and are used to measure the quality of the service or system. SLOs are used to determine whether a service is meeting the expectations of its users, and to identify areas where the service can be improved.

    SLOs are typically expressed in terms of service level indicators (SLIs), which are metrics that are used to measure the performance of a service or system. Some examples of SLIs include availability, response time, and error rate. SLOs are often defined in terms of these SLIs, such as specifying a target availability or response time for the service.

    In order to ensure that a service or system is meeting its SLOs, the performance of the service or system is regularly monitored and tracked using the appropriate SLIs. If the service or system fails to meet its SLOs, appropriate actions can be taken to improve its performance.

## SLI
    - Service Level Indicators (SLIs) are metrics that are used to measure the quality of a service or the performance of a system. They are often used in the context of service level agreements (SLAs), which are contracts that define the level of service that a customer can expect from a provider. SLIs help to monitor and track the performance of a service or system, and ensure that it is meeting the requirements defined in the SLA. Some examples of SLIs include availability, response time, and error rate.

## SLA
    - A service level agreement (SLA) is a contract between a service provider and a customer that specifies the level of service that the provider will deliver. The SLA outlines the specific services that the provider will offer, the performance standards that the provider will meet, and the terms and conditions that apply to the delivery of those services. SLAs are commonly used in the context of information technology (IT) and telecommunications, but they can also be applied to any service-based industry. The goal of an SLA is to provide a clear and detailed understanding of the service that the customer can expect, and to establish a framework for measuring and managing the quality of that service.

## Error Budget
    - An error budget is a concept used in the discipline of Site Reliability Engineering (SRE) to manage the trade-offs between reliability and development velocity. An error budget is a fixed amount of downtime or degraded service that is allocated to a system over a given time period. This budget is intended to allow teams to continue deploying new code and features without constantly worrying about the potential impact on system reliability. The error budget is monitored and managed by the SRE team, and when the budget is exhausted, the team will take action to improve the system's reliability before allowing further development. The goal of using an error budget is to balance the need for rapid development with the need for high reliability, and to allow teams to iterate quickly and innovate without sacrificing the overall reliability of the system.

## Toil
    - In the context of Site Reliability Engineering (SRE), toil refers to work that is manual, repetitive, automate-able, and that does not add business value. Toil is a drain on an SRE team's time and resources, and it can prevent them from focusing on more important tasks that add value to the organization. Toil can include tasks such as responding to alerts, handling routine maintenance, or manually provisioning infrastructure. The goal of SRE is to reduce toil as much as possible by automating repetitive tasks and eliminating low-value work, so that SRE teams can focus on tasks that are more important and valuable.

## Exceptions
    - Checked and Unchecked
        - Throws, Throw, Throwable
