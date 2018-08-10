# ORCA-Modernization

This repo contains documentation describing the Alaska Department of Health and Social Services, Office of Children's Services (OCS) modernization project. It is intended to be a place where project participants can keep track of the overall project goals, the decision framework, progress to date and learnings as we work. It is also intended to be a project home page where members can access important and up-to-date project information that exists somewhere else.

## Project Vision

Alaska OCS is developing a modern Comprehensive Child Welfare Information System (CCWIS) that enables staff to more efficiently provide services to children in need, integrate with other state agencies, and comply with the latest [federal requirements](https://www.law.cornell.edu/cfr/text/45/1355.52) for child welfare systems. Using [agile development](https://modularcontracting.18f.gov/agile-development/) and [modular procurements](https://modularcontracting.18f.gov/modular-procurement/), OCS has the goal of implementing a CCWIS system that not only meets state and federal standards, but is user-friendly for our clients, OCS staff, and state technical staff.

## Objectives

The initial procurement for this effort will focus on workload Dashboards for targeted users of the system. Initially, the Dashboard effort will serve as the .NET pilot project, and for building a new API and API connections points. 

This initial focus will help the product team to:

* Deliver value quickly to end users.
* Identify a technical strategy that will support OCS efforts to enhance the system for end users, and align with the requirements of CCWIS
* Support the build out of a fuller product roadmap, to communicate to users and stakeholders the future direction of the project.
* Allow OCS and 18F to "road test" both a modular procurements strategy and a DevOps infrastructure for working with vendors.
* de-risk efforts to migrate to .NET by prototyping

## Near-term Milestones

- [x] Begin organizing work in sprints and conducting regular agile ceremonies.
- [x] Identify users that can participate in research sessions to help prioritize needs for initial mobility effort.
- [x] Begin technical assessment of existing ORCA system .
- [ ] Put in place initial build and deployment pipeline for ORCA code (in progress). 
- [ ] Develop initial version of product roadmap. (in progress)
- [ ] Identify opportunities to prototype and de-risk initial procurements. (not yet started)

## Strategies

### Encase ORCA

We will identify a portion of ORCA’s functionality that can be modernized, balancing the need for adding functionality that’s of high value on mobile devices against the feasibility of opening access to that ORCA functionality within the existing Java structure. Then the existing functionality will be rewritten in a new, modernized module, using the software environment of OCS’s choosing (e.g., C# on .NET), using a responsive design (perhaps even as a progressive web app), to provide robust support for all possible clients. Finally, the old, now-redundant functionality will be eliminated.

### Adopt agile practices

Working in tightly-scoped sprints to incrementally enhance the existing child welfare system will be a key to the success of a modular procurement strategy. Adopting agile practices early, even before a vendor is engaged and code is shipped, will ensure that OCS has the capacity to successfully engage with vendors. 
 product roadmap, OCS staff and 18F will identify discrete modules that can be encapsulated into modular procurements - narrow low-risk acquisitions that can be used to incrementally modernize the existing child welfare system. Developing this strategy will entail identifying interested vendors that are proficient in agile software development, building out technical prototypes to validate issues and lower risk, and working to continually improve the overall acquisition strategy through the application of agile principles like continuous improvement.

### Put in place a DevOps infrastructure

Before OCS can adopt a modular procurement strategy and adopt agile practices, it needs to develop a capacity to accept work delivered in an iterative fashion. Adopting DevOps practices and constructing a delivery pipeline are essential to the successful adoption of agile practices.

### Develop a Product Roadmap

Develop a product roadmap to guide the efforts of OCS staff and to communicate to vendors and other stakeholders the near and long-term objectives of the project. The product roadmap will be used to identify different modules and components that can be targeted for modular procurements to build out the new CCWIS system incrementally. The product roadmap will be a living document, updated frequently to reflect learnings from procurements, changing priorities and input from stakeholders.

## Risks 

* Ensuring a focus on end users. There may be a strong incentive to develop a CCWIS system provided by the new regulations promulgated by DHSS/ACF. Ensuring the effort to modernize the existing system is focused on delivering value to end users will require effort on the part of OCS and 18F. 
* Complia
### Develop a modular procurement strategy

Using thence with CCWIS. Future funding from ACF is linked to compliance with CCWIS requirements, and ORCA modernization / enhancement efforts will need to help OCS achieve this goal.
* Feasibility of encasement strategy. It is currently unknown how feasible 18F's standard "encasement" approach to legacy modernization is for the existing ORCA system.
* ORCA contains considerable technical debt, [as documented](TechnicalDebt.md).
* See [Technical Risks](TechnicalRisks.md) for more.

## Ongoing Strategic Issues

* Identifying vendors that are proficient in agile practices to bid on modular contracts.
* Determining whether partial changes to existing ORCA system will be sufficient to achieve project goals, or if more wholesale modifications / updates will be needed.

## Contributing to this repo
* Read the [CONTRIBUTING](/AlaskaDHSS/ORCA-Modernization/blob/master/CONTRIBUTING.md) Policy
* Questions or suggestions? Open a [new issue](/AlaskaDHSS/ORCA-Modernization/issues) to ask or suggest.
* Want to send us a change? Create a new [pull request](/AlaskaDHSS/ORCA-Modernization/pulls).
