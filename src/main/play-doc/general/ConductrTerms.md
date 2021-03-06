# ConductR terms

Term        | Description
         ---|---
Agent       | The ConductR executor
Application | A collection of one or more bundles representing a meaningful business purpose. A Developer determines what constitutes an Application. Lightbend ConductR recognises the aggregation of bundles through a "system" attribute assigned to the bundle. This attribute can be used by a component to associate themselves with an Akka cluster (for example).
Bundle      | A bundle is an archive of components along with meta data (a bundle descriptor file) describing how the files should be executed. Bundles are similar to executable JARs with the difference being that they are not constrained to executing just JVM code. Bundles are also named using a digest of their contents so that their integrity may be assured. Bundles represent a unit of software that may have a release cycle which is distinct from other bundles.
Component   | A bundle can have many components although it typically has just one. A component in Lightbend ConductR represents a unit of software that  describes what will become a process when a bundle is started.
Configuration | Configuration alters a component's behavior at runtime and may declare the location of a database, credentials, logging file levels and so forth. Configuration is primarily sourced from within a bundle's components. In addition external configuration may be applied across all of a bundle's components when a bundle is loaded. This additional configuration would typically relate to values for production, testing and so forth.
Core        | The ConductR scheduler
Developer   | Developers who develop using Scala/Java, Akka, Play and/or other Lightbend technologies.
Operator    | Targets the "Linux admins" of the Ops world and covers both IT Ops and Dev Ops style roles.
Service     | An Application can be broken down into logical services, comprised of generalised services or not even have services. What constitutes a service is left to the Developer. Lightbend ConductR recognises the aggregation of bundles through a "system" attribute assigned to the bundle. This attribute can be used by a component to associate itself with an Akka cluster (for example).
