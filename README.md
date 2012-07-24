Ganger - A simple automate tool.
===============

What is Ganger
--------------

Ganger is a simple automate tool. It can automate deploy packages, launch
target processes, update packages deployment(kill the old process and launch
the new one), restart target processes and monitor the status of target 
process.

It saves your time for development, and make it easier to deploy your systems
on many target machines simultaneously.


Features
--------

Automatation: help you do some automate tasks, for example: deploy packages,
start processes, stop processes and update deployments etc.
(Note: deploy action *ONLY* support compressed binary executables(.tar.gz)
currently.)

Lifecycle management: you can start, stop, restart or update the target
process.

Dependence management: we organize the package as a directed graph with no
cycles, when a process of a package crashed or started, the processes of the 
package which depend on it will be notified. Automate action will operate on 
packages as the topological order of the dependence graph(or reverse order for 
actions similar to #stop#).

Status monitor: monitor the target process's status.