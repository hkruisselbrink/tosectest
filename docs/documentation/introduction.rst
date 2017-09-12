Introduction
============
EFF stands for EasyFlexibleFramework.

It is an event based framework combined with QObject wrappings use to create an extensible application platform in C++. 
Various subprograms can be developed around this framework in Lua. Each subprogram (or "mode") consists of multiple Lua modules.
An EasyObject application (referred to as the EFFHostApplication) can be given the EFF layer by exposing the LuaCaller functionality 
through a context menu which allows the user to call an EFF mode script which in turn will determine the host application's functionality.
The key difference between EFF and simple lua script calling resides in two aspects.

1. EFF is a persistent process, it runs as long as the application is running.
2. Signals and events can be connected to EFF and responded to from within the EFF layer.

EFF Principle
-------------
The principle on which EFF is based is to provide and open, flexible and most of all simple, tidy and syntactically-friendly API for 
anyone who wishes to create a specific application based on the mechanisms the HostApplication provides.

EFF Components
--------------

- Main
- Interface and FunctionSet
- Modes
- Modules
- Libraries