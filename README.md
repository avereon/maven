# Xeomar Maven Parent POMs

This project maintains the parent poms used by the Xeomar group. The parent poms
define common configuration, resources and definitions for all Xeomar projects.

## POM Hierarchy

- top - The top pom where most plugin versions are defined
  - asm - The assembly project that defines common assembly descriptors
  - jar - The parent pom for jar projects and jar-like projects like products 
  and mods.
    - prd - The parent pom for products
      - prg - The parent pom for programs
      - mod - The parent pom for modules
- web - The parent pom of web projects. The parent of web projects is the 
  spring-boot-parent pom and not the Xeomar top pom.

## Builds

This project is configure for automatic build and deployment, just like any 
project. This ensures that changes to the poms are deployed in a timely fashion
and that dependent projects are rebuilt when the parent poms change. 
