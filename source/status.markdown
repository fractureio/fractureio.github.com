---
author: 7sharp9
layout: page
title: "status"
date: 2012-02-03 21:41
comments: true
sharing: true
footer: true
---
## Upcoming feature set
This is more or less a brain dump of the proposed new features.

### Remote Agents
   * agent.Start("localhost", 4567, async{...}) 
   * Agent repository access - transparent agent access
   * Unique identifies applied to agent
   * One shot and persistant Spawn{} workflows
   * Control messages for agents - (Shutdown, RestartComms, poison-pill, Kill, Hot-swap)
   * Out of reach message buffering 
   * Authentication 
   * Expand AsyncReply to remote agents 

### Fhin
Message compaction library for remote agents
   * Records
   * Discriminated unions
   * primitive types

### Overseers 
Expand Control messages for overseers
   * Watch
   * Unwatch
   * Spawn
   * Error-strategy
   * Allowable-failures
   * Restart-on-failure
   * max-failure-number
   * failure-interval

### Distributers
   * Context run changer 
   * Pressure behaviour
   * Abort
   * Discard newest
   * Discard oldest
   * Discard low priority
   * Throughput limiting 
   * Expand Control messages for dispatchers 

### Pools/agency
   * Pool changing algorithms - linear increase pressure, mean-increase pressure 
   * Distribution algorithms - Round-robin, load based, content based 
   * Throughput limiters 
   * Expand Control messages for pools 

## Platform work

   * use of libuv for multi-platform speed
   * Leverage new Feature of Windows Vista/7/8 
   * Tcp API enhancements in Vista
   * Out of the box support for standard .NET web platforms such as WebForms and MVC - See FastCGI or fcgi-mono-server Frank, ServiceStack
  