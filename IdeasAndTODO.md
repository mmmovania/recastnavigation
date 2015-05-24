# Ideas #

  * Automatic hide point/segment generation
  * Automatic jump link generation
  * Create waypoint graph instead of navmesh
    * from regions
    * from depth field skeleton
    * distribute waypoints uniformly
    * disc based navigation generation (vrlab.epfl.ch/~jpettre/publis/05vcrowdpettre.pdf)

# TODO #

  * Profile memory usage
  * Profile largest bottlenecks
  * Speed up rasterization
    * all integer
    * SSE
    * calc min/max per Y span to prevent extra work
  * Fix detour A-star heuristic
    * use float as cost, not short (and profile mem/perf change)
    * adjust start/end poly center to be start/end point