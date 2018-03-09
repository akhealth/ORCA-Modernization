# Technical Risks

The following is a living document of the technical risks associated with the ORCA Modernization project. 

## Encasing ORCA is an unknown

ORCA has no API. The amount of effort required to modify its internal functionality to encase it and interface with it is simply unknown at this point. It is certainly _possible_—OCS has control over all of the code that comprises ORCA—but there’s not yet any way to know whether it will be viable compared to other options (e.g., greenfield development).

## There is no prototype

No internal work has been done to “de-risk” the proposed scope of work, such as by building a prototype of the product planned for the first procurement, so we don’t know all of the technical risks.

## Logic may not be centralized

It's not clear how much logic is present in the database (e.g. stored procedures) and how much is in the Java. This may complicated encasement.

## Lack of mobile device standardization

There are no standard-issued mobile devices for OCS staff (e.g. iPhones), which makes it difficult to ensure that all users of the system have a quality experience. Relatedly, DHSS lacks mobile device management infrastructure to enforce minimum security standards for the mobile devices that are in use.

## Inconsistent mobile service

Spotty mobile coverage in rural Alaska makes it a challenge to provide a mobile experience that works reliably and consistently.

## DHSS is new at DevOps

It’s only over the past year that DHSS has adopted DevOps within its technical culture, and only started using it with a vendor in January. While that adoption has been aggressive and capable, it is still limited in duration and scope.

## DHSS IT is stretched thin

The agency’s IT positions are not fully staffed. Insofar as it is necessary for DHSS to provide technical support for this work, that presents a risk to the work being done in a timely manner.
