---
title: "Node, Javascript - Garbage Collection"
categories:
  - Javascript
  - Node
tags:
  - Javascript
---
This post is a summary for [The modern Javascript Tutorial](https://github.com/javascript-tutorial).

## Reachability
The main concept of memory managament in JavaScript is Reachability.  
Reachable values are those that are accessible or usable somehow. They are guaranteed to be stored in memory.
- Root 
  - Local variables and parameters of the current function
  - Variables and parameters for other functions on the current chain of nested calls.
  - Global variables

## Internal Algorithm
- mark-and-seep
  - The garbage collector takes roots and “marks” (remembers) them.
  - Then it visits and “marks” all references from them.
  - Then it visits marked objects and marks their references. All visited objects are remembered, so as not to visit the same object twice in the future.
  - …And so on until every reachable (from the roots) references are visited.
  - All objects except marked ones are removed.
- Optimizations
  - Generational Collection: Split obejcts to "new ones" and "old ones". Clean up new ones aggressively
  - Incremental Collection: Do not try to mark whole objects. Split the garbage collection into pieces
  - Idle-time Collection: Garbage collector runs only while the CPU is idle
