---
layout: post
title: Clean Code (SOLID)
author: Aristotelis Pozidis
date: '2021-02-17 16:42:50 +0530'
category: guides
summary: The only thing that is constant is change!
thumbnail: solid.png
---

We must create elegant and robust software, we must keep in mind that the software is never dormant, it always keeps changing.

As Heraclitus said “The only thing that is constant is change”

So by applying the **SOLID** principles, we achieve more flexible, easily maintainable, and readable code. 
There are 5 main rules that make the **SOLID** each for every letter of the word,

S	→ (`SRP`)	Single Responsibility Principle.

O	→ (`OCP`)	Open Closed Principle.

L	→ (`LSP`)	Liskov Substitution Principle.

I	→ (`ISP`)	Interface Segregation Principle.

D	→ (`DIP`)	Dependency Inversion Principle.

## SRP
Every software component should have one and only one responsibility.
A component can be a class, a method, or a module.

  • Cohesion → Is the degree to which various parts of the software are related.

  • Coupling → Is defined as the level of dependency between various software components.

Higher cohesion and loose coupling attain better adherence to the `SRP`

Every software component should have one and only one reason to change.

## OCP
Software components should be closed for modification, but open for extension.

  • Closed for modification → Adding new features should NOT modify existing code.

  • Open for extension → A software component should be extendable (new feature or behavior).

Ease of adding new features (E.g. with Interface that is implemented)
This leads to the minimal cost of developing and testing software.
`OCP` often requires decoupling, which in turn automatically follows the `SRP`.

## LSP
Objects should be replaceable with their subtypes without affecting the correctness of the program. Use the “Is-A” way of thinking. (But not always E.g Hen is-A Bird)
Solutions to fix your design:

  • Break the hierarchy

  • “Tell don’t ask.”

## ISP
No client should be forced to depend on methods it does not use.
Segregate all the SUPER interfaces. Use smaller more specific ones.

Violations of `ISP`:

  • Fat(Super) Interfaces.

  • Interfaces with Low Cohesion.

  • Empty Method Implementations.

## DIP
High-level modules should not depend on low-level modules. Both should depend on abstractions.
Abstractions should not depend on details. Details should depend on abstractions.
Use Dependency Injection to achieve this. There are Inversion Of Control frameworks as well like Spring (`IOC` container).

## About the **SOLID** Principles

**SOLID** principles are all intertwined and interdependent.
**SOLID** principles are most effective when they are combined together.
It is important to get a wholesome view of all the **SOLID** principles.

**SOLID** principles complement each other, and work together in unison, to achieve the common purpose of well-designed software.
