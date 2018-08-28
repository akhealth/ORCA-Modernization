## Modular procurements

-   In accordance with our [modular acquisition approach](#) and consistent with [best practices for technology procurements](http://farsite.hill.af.mil/reghtml/regs/far2afmcfars/fardfars/far/39.htm#P34_5241),
    OCS will be modernizing the ORCA system through a series of
    relatively-smaller procurements for well-defined feature sets.

-   Through these procurements, we will move towards a more
    loosely-coupled approach to system development, working with
    vendors to develop independent, interoperable modules with clearly
    defined service interfaces.

-   Different vendors may build different components of the ORCA system,
    while users will continue to interact with a unified experience.

## Encasement pattern

-   In adopting this more modular approach, we also open ourselves to
    utilizing the encasement pattern to support incremental
    modernization of ORCA.

-   The encasement pattern will support the development of new feature
    sets in a way that is decoupled from the existing legacy system,
    allowing components of the existing ORCA system to be
    decommissioned in a way that is visible to the end users.

-   New features and functionality will access data in the existing ORCA
    system via a proxy layer built on top of the State of Alaska’s
    existing Enterprise Service Bus (ESB) platform.

-   Vendors should not be required to understand or support existing
    systems, but rather should interact with existing systems through
    well defined and well documented APIs.

-   Service endpoints used to enable new functionality will be built out
    as they are needed, to support ongoing development, rather than
    all at once prior to work on new features and functionality. This
    will help speed the delivery of new features to end users and help
    avoid premature optimization.

## Migrate to .NET

-   DHSS is moving towards establishing the .NET stack as standard
    platform for new application development.

-   We are targeting:

    -   [Microsoft
        C\#](https://docs.microsoft.com/en-us/dotnet/csharp/) for
        application programming language

    -   [Microsoft Dotnet Core](https://www.microsoft.com/net) for
        application framework

    -   [Microsoft Azure App
        Service](https://azure.microsoft.com/en-us/services/app-service/)
        Platform-as-a-Service for application environments

    -   Utilizing the State of Alaska's existing ESB for accessing
        on-premises data sources.

-   We are open to exploring the use of different front-end technologies
    and tools, but will favor those components that have been [used
    in other recent DHSS
    projects](https://github.com/AlaskaDHSS/Dpa-Eisr-UnifiedSearch/blob/staging/web/package.json)
    to support a more unified technical approach.

## Moving to cloud / Azure

-   DHSS has established Microsoft Azure as it’s designated cloud
    platform, and Azure App Service as it’s Platform-as-a-Service
    offering.

-   OCS will adopt Microsoft Azure, and will utilize [Azure App
    Service](https://github.com/AlaskaDHSS/DevSecOpsMvp/tree/master/appservice)
    (to the extent practicable) for the ORCA system modernization
    project.

-   Following our modular approach, new functionality will be built in
    the .NET technology stack and deployed to Azure.

-   [VSTS](https://github.com/AlaskaDHSS/DevSecOpsMvp/tree/master/vsts)
    will be used to manage the work of the product team and vendors.
    [Git](https://visualstudio.microsoft.com/team-services/git/)
    will be used as the version control system, and all work will be
    deployed to Azure via a [continuous
    delivery](https://docs.microsoft.com/en-us/azure/devops/what-is-continuous-delivery)
    pipeline.

## DevOps - New project delivery

-   We rely on DevSecOps for automation and monitoring of code
    integration, testing, and deployment.

-   Our DevSecOps pipeline is built atop VSTS for deployment to Azure.

-   We practice continuous integration, continuous deployment, and
    continuous testing (including security testing).

-   All new code has tests developed simultaneously, with cumulative
    test coverage of not less than 90%.

-   New projects built on Azure will adopt automated DevOps methods from
    the start

-   OCS will provide vendors with the ability to deliver working
    software from Sprint 1.

-   OCS will involve Security along the way, understanding that the goal
    is to frequently get working, in-progress software into the hands
    of real users to use in real life situations

## DevOps - Existing ORCA

-   The existing ORCA build and deployment process is semi-automated and
    uses an internally developed tool that has not been actively
    maintained; the original developer is no longer with the project
    and there is no expertise to maintain it.

-   For every build, the user is still required to manually select
    artifacts that need to be included in it.

-   OCS is in the process of updating these build and deployment methods
    with the goal of achieving a fully automated DevOps approach for
    the existing ORCA product

-   Existing ORCA code is being migrated to git, and the existing build
    steps which are encapsulated in their legacy build tool are being
    extracted to support a new VSTS → Azure build and deployment
    pipeline for new features developed through the modular
    acquisition approach.

## Technical prototyping

-   Especially when working with legacy systems, it's important to test
    technical assumptions before scoping any kind of procurement
    because there are almost certainly unknown hazards that can put
    your procurement at risk.

-   Prototyping a small end-to-end user flow should help identify any
    hazards in the code, the deployment process or any other technical
    aspect of a project. This will help teams properly scope the
    procurement and build out a reasonable RFP with some useful
    documentation for buyers and for vendors.

-   Unlike most kinds of prototypes, technical prototypes are not
    focused on user experience, but rather on the mechanics behind the
    user's experience. They show just enough of the user-facing
    functionality to verify some kind of technical implementation.


