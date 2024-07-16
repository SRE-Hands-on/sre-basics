# What is SRE (Site Reliability Engineering)? 

"Site reliability engineering (SRE) is a software engineering approach to IT operations. SRE teams use software as a tool to manage systems, solve problems, and automate operations tasks." [Red Hat](https://www.redhat.com/en/topics/devops/what-is-sre)

Site Reliability Engineering (SRE) incorporates aspects of software engineering and applies them to infrastructure and operations. The primary goal of SRE is to create scalable and highly reliable software systems. To support you on this journey, some concepts are crucial to give you the right tools to your daily activites.

## Network and TLS

Network concepts and TLS are essential for SRE as they form the backbone of secure, reliable and efficient service delivery.

[Network and Security] (https://github.com/SRE-Hands-on/network-and-security) - See a bit depper concepts on this repo


## Coding and Testing

Writing, reviewing, and maitaining code to support infrastructure operations and ensuring changes are reliable and do not introduce new issues.

## CI/CD

### Continuous Integration (CI)

Continuous Integration is a development practice where developers integrate code into a shared repository frequently, ideally several times a day. Each integration is verified by an automated build and automated tests.

##### Key Points:

**Automated Testing**: Ensures that the code is functional and does not break existing functionality. This includes unit tests, integration tests, and sometimes system tests.

**Automated Builds**: Each commit to the repository triggers an automated build, ensuring that the software can be compiled and packaged.

**Early Detection of Issues**: Frequent integrations help detect and resolve issues early, reducing the time and effort required to fix bugs.

**Code Quality**: Maintaining high code quality through linting and static code analysis.


### Continuous Delivery (CD)
Definition: Continuous Delivery is a software development practice where code changes are automatically prepared for a release to production. This ensures that the software can be released at any time.

#### Key Points:

**Automated Deployment Pipelines**: Automating the deployment process, including stages like staging, testing, and production, to ensure consistency and reliability.

**Testing in Production-like Environments**: Ensuring that code is tested in environments that closely resemble production to catch environment-specific issues.

**Rollback Mechanisms**: Implementing automated rollback procedures to quickly revert to a previous stable state in case of deployment failures.

**Incremental Updates**: Deploying small, incremental changes to minimize the risk of large-scale failures and to make troubleshooting easier.


### Continuous Deployment (CD)

Continuous Deployment takes Continuous Delivery a step further by automatically deploying every change that passes the automated tests to production.

#### Key Points:

**Fully Automated Deployments**: Every change that passes all stages of the deployment pipeline is automatically deployed to production without human intervention.

**Monitoring and Alerting**: Extensive monitoring and alerting systems to detect and respond to issues as soon as they occur in production.

**Feature Flags**: Using feature flags to control the exposure of new features to users, allowing for safe and gradual rollout.

**Resilience and Recovery**: Building systems that are resilient to failures and can recover quickly through mechanisms like auto-scaling, redundancy, and self-healing.


### CI/CD Pipeline 
An effective CI/CD pipeline typically includes:

**Source Code Management**: Using tools like Git to manage source code.

**Build Automation**: Tools like Jenkins, Travis CI, or CircleCI to automate the build process.

**Automated Testing**: Incorporating various testing frameworks and tools to automate testing.

**Artifact Management**: Using artifact repositories like Nexus or Artifactory to manage build artifacts.

**Deployment Automation**: Tools like Spinnaker, Kubernetes, or Terraform to automate the deployment process.

**Monitoring and Logging**: Implementing robust monitoring and logging solutions like Prometheus, Grafana, ELK Stack, or Datadog.

**Security Scanning**: Integrating security checks within the pipeline to ensure compliance and security standards.

By leveraging CI and CD practices, SRE teams can ensure that software is delivered quickly, reliably, and securely, meeting the high standards of availability and performance required in modern software systems.

## Containers (Docker, Podman, containerd)

Contaienr are a lightweight, portable and self-suficient units that encapsulate an application and all its dependencies, so it can run consistently across differenct computing environments

It has three key characteristics:

- **Isolation**: Container provide process and filesystem isolation using features like namespaces and control groups(cgroups) in the Linux kernel.
- **Portability**: Container can run on any system that supports containerization, ensuring that applications behave the same regardless of where they are deployed.
- **Efficiency**: Containers share the host OS kernel, making them more lightweight than virtual machines, wich include separate OS instance for each VM.



## Orchestration (Kubernetes, Nomad, OpenShift and etc)
In progress.

## Configuration Management
In progress.

## Reliability and Availability
In progress.

## Monitoring and Alerting
In progress.