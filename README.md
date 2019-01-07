# SAFER Principles for Javascript

A summary of principles we want to use to create safer Javascript services.

## Disclaimer

This is a work in progress draft of principles and guidelines we think of being good for developing libraries/services/modules that integrate in hogher order components, applications, services or systems of these.

We do not claim these practices to be a "best practice" and will not be held responsible for any damages, harms or losses, that have been caused by following these principles.

Use at your own risk.

## Naming

##### Program

We will summariz all the terms application/package/module/lib/service and so on as "program" mainly because their lowest common factor is that code is somehow executed.

## Principles

The term SAFER is derived from the word safe which here refers to safety in terms of "unintrusiveness" in relation to the surrounding environment. A programm is thus safe when it

* works as intended
* works in compliance to the surrounding environment
* not mutates logic, flow, code or data of it's consumers or environment
* provides extensive control over it's behavior
* is unopinionated about the way it is integrated, executed, deployed or operated
* keeps the lowest profile that is possible in context of it's purpose

### Standards

Use and support standards where possible and reasonable.

*Internally* this means to use code quality standards or consider standards of security.

*Externally* this means to provide configurations that allow compliance to regulations, laws or international standards.


### Advanced control

Give devevelopers as much as control as they will need. While this will result in more work for developers, they will also have the freedom to configure and stay in control. 

Provide the control in a way, that developers can secure the control procedures.

### Freedom and felxibility

It should always be easy to integrate, change and scale a program. However, freedom to choose how to integrate, deploy and operate a program should be of higher priority.

### Economically and ecologically balanced

The program should aim to use as few code, space, memory and cpu as possible but not in the expense of functionality and configurability.

### Respect and responsibility

The program has to respect the design and execution of it's consumers and surrounding environment. Thus it is design to be "receiving" and won't alter any of your code. No namespace pollution, no injections, no hooks. The responsibility of integration remains to the developer

## When not to use SAFER

The SAFER principles are mainly targeting programs that are part of other programs, like libraries, services, modules, packages etc.

It may not be suitable for the higher and highest levels of an architecture, where certain restrictions are necessary to provide a consistent and secure environment.
