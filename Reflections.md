# CarND-Controls-MPC Reflections
Self-Driving Car Engineer Nanodegree Program
---

## Latency

Latency is implemented in this project via the supplied thread sleep_for instruction (main.cpp:186). Although tricky, the sleep command is a requirement to better represent real-world conditions and performance. The actual effect of this code makes it necessary to commit changes that prevent actuations from being applied a timestep too late (lines 113-116 and 76).
