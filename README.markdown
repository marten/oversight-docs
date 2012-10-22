Server Monitoring and Metrics
=============================

What is the difference between server (cluster) monitoring, application
monitoring and application metrics? I think little. Why is it that it seems
like every single monitoring app or service out there sucks in it's own
way? Could we do something like Travis does, where every part of this system
is open source, yet it's still interesting as a service for people who don't
want to spend effort getting everything working?

Main parts of the architecture:

* *Agent*
  An agent is software that runs on each monitored machine. The agents
  periodically checks things on their machines and reports their values to the
  collector.

* *Collector*
  The collector is a central piece of the architecture that receives values of
  checks sent by the agents.



Feature wishlist
----------------

* Every morning send out a "sitrep" that lets you know how the day went.
  This is useful to be notified about issues that are not mission critical
  and thus weren't immediately notified about.
