nodejs-munin
============

A [Munin](http://munin-monitoring.org) stats catcher & plugin for node.js applications.
Allows node.js apps to collect stats and report them on-demand to a [Munin](http://munin-monitoring.org) node.

Inspired by [StatsD](https://github.com/etsy/statsd). StatsD uses Graphite, but I had an existing Munin-based graph infrastructure, so this works with Munin.

Still under development. Code was copied from a site where it's used in production, but is not yet generic enough for common use.

Example [munin plugin](http://munin.readthedocs.org/en/latest/plugin/use.html#configuring) configuration:
```
[munin_nodejs_*]
env.statsHost 127.0.0.1
env.statsPort 8082
env.statsPath /stats
```

By [Ben Buckman, New Leaf Digital](http://newleafdigital.com)
