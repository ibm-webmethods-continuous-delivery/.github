# IBM webMethods Continuous Delivery Accelerators

This GitHub public organization contains a number of repositories offering contextual accelerators for software delivery using webMethods. These accelerators may refer to any product and any version in the suite. They are to be considered as "after-market" additions to the product and not in substitution of existing product capabilities.

All repositories within follow the same rules and licensing. License is always [Apache 2](https://www.apache.org/licenses/LICENSE-2.0).

This organization is intended for consumption from customers and partners that pursue continuous delivery practices when deploying and operating webMethods based landscapes. It is driven by a group of customer-facing IBM consultants, however it has also been receiving external contributions too.

The accelerators present here are intended to be a starting point "solution zero", on one hand, and focused solutions to typical specific situations, on another. They are offered as-is with no warranty whatsoever, it is the responsibility and accountability of the user to appropriately increment, test and assure the derived solutions for their own purposes.

## Concept and Ground Rules

The organization's accelerators are built for continuous delivery. Here, we take [Dave Farley's and Jez Humble's definition](https://continuousdelivery.com/) as an organization ability to always keep the software in a deployable state.

> Continuous Delivery is the ability to get changes of all types—including new features, configuration changes, bug fixes and experiments—into production, or into the hands of users, *safely* and *quickly* in a *sustainable* way.

A detailed description of the framework used in this organization can be found in the [1c-framework](https://github.com/ibm-webmethods-continuous-delivery/1c-framework) repository.

Contributors should observe the [contributing](https://github.com/ibm-webmethods-continuous-delivery/.github/blob/main/CONTRIBUTING.md) and [code of conduct](https://github.com/ibm-webmethods-continuous-delivery/.github/blob/main/CODE_OF_CONDUCT.md) guidelines before submitting increments of any nature. These guidelines are evolved from IBM's rules observable in the [repo-template](https://github.com/IBM/repo-template) repository.

## Structure

The capabilities offered are intended to be used with some degree of autonomy and are grouped in the following "chapters". Each chapter has a prefix of two chars, allowing the users to understand immediately wht type of capability is contained in the repository:

Prefix|Area
-|-
1c-|Concept and Framework
2l-|Code libraries
3p-|Prerequisites
4h-|Technology Assets Procurement
5s-|Integration Service with Continuous Delivery
6o-|GitOps style Continuous deployment


### Concept and Framework (prefix `1c-`)

This area contains fundamental principles and ideas that guide and organize this organization.

### Code Libraries (prefix `2l-`)

These are pure code libraries, that are abstracting important aspects used in the other areas.

### Prerequisites (prefix `3p-`)

For ease of access, the simplest way to use these artifacts is by having a docker compose enabled workstation or laptop. Docker compose is preferred in front of other technologies like Podman, Kubernetes or OpenShift due to the fact it is the lightest way to run development run configurations locally and its popularity. The final destination for delivery remains a proper containerization orchestrator. The authors are using Rancher Desktop on Windows 11 workstations and this is considered  the fundamental way of working.

With time, specific deployments are continuously added, for example resources to showcase the appropriate utilization of Azure pipelines, GitHub actions or AWS code pipelines. Prerequisites repositories may include, for example, Terraform artifacts to help with provisioning of Azure DevOps cloud resources or AKS / EKS setup, or private links set up examples and so on.

### Technology Assets Procurement (prefix `4h-`)

This contains code that automate download of product binaries, qualification of container images and building of custom images.

### Integration Services with Continuous Delivery (prefix `5s-`)

This area represents the main purpose of the overall exercise.
Development repositories are Github templates, intended to be easy to replicated by webMethods developers.
These repositories deliver either built code packages or container images.

### GitOps Style Continuous Deployment (prefix `6o-`)

This area contain GitOps style examples for delivery towards non-local, scalable production like environments.
