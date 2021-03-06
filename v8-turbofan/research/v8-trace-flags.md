### DataTypes

```
--track-fields (track fields with only smi values)
      type: bool  default: true
--track-double-fields (track fields with double values)
      type: bool  default: true
--track-heap-object-fields (track fields with heap values)
      type: bool  default: true
--track-computed-fields (track computed boilerplate fields)
      type: bool  default: true
--track-field-types (track field types)
      type: bool  default: true
--trace-block-coverage (trace collected block coverage information)
      type: bool  default: false
```

### TurboFan

```
--trace-concurrent-recompilation (track concurrent recompilation)
      type: bool  default: false

--trace-turbo (trace generated TurboFan IR)
      type: bool  default: false
--trace-turbo-graph (trace generated TurboFan graphs)
      type: bool  default: false
--trace-turbo-scheduled (trace TurboFan IR with schedule)
      type: bool  default: false
--trace-turbo-cfg-file (trace turbo cfg graph (for C1 visualizer) to a given file name)
      type: string  default: nullptr
--trace-turbo-types (trace TurboFan's types)
      type: bool  default: true
--trace-turbo-scheduler (trace TurboFan's scheduler)
      type: bool  default: false
--trace-turbo-reduction (trace TurboFan's various reducers)
      type: bool  default: false
--trace-turbo-trimming (trace TurboFan's graph trimmer)
      type: bool  default: false
--trace-turbo-jt (trace TurboFan's jump threading)
      type: bool  default: false
--trace-turbo-ceq (trace TurboFan's control equivalence)
      type: bool  default: false
--trace-turbo-loop (trace TurboFan's loop optimizations)
      type: bool  default: false
--trace-alloc (trace register allocator)
      type: bool  default: false
--trace-all-uses (trace all use positions)
      type: bool  default: false
--trace-representation (trace representation types)
      type: bool  default: false


--turbo-stats (print TurboFan statistics)
      type: bool  default: false
--turbo-stats-nvp (print TurboFan statistics in machine-readable format)
      type: bool  default: false

--trace-turbo-inlining (trace TurboFan inlining)
      type: bool  default: false


--trace-osr (trace on-stack replacement)
      type: bool  default: false

--trace-environment-liveness (trace liveness of local variable slots)
      type: bool  default: false

--trace-turbo-load-elimination (trace TurboFan load elimination)
      type: bool  default: false
--trace-store-elimination (trace store elimination)
      type: bool  default: false
```

### Ignition

```
--print-bytecode (print bytecode generated by ignition interpreter)
      type: bool  default: false
--print-bytecode-filter (filter for selecting which functions to print bytecode)
      type: string  default: *
--trace-ignition-codegen (trace the codegen of ignition interpreter bytecode handlers)
      type: bool  default: false
--trace-ignition-dispatches (traces the dispatches to bytecode handlers by the ignition interpreter)
      type: bool  default: false
--trace-ignition-dispatches-output-file (the file to which the bytecode handler dispatch table is written (by default, the table is not written to a file))
      type: string  default: nullptr

--code-comments (emit comments in code disassembly; for more readable source positions you should add --no-concurrent_recompilation)
      type: bool  default: false
```

### Garbage Collector

```
--trace-track-allocation-sites (trace the tracking of allocation sites)
      type: bool  default: false
--trace-migration (trace object migration)
      type: bool  default: false

--trace-gc (print one trace line following each garbage collection)
      type: bool  default: false
--trace-gc-nvp (print one detailed trace line in name=value format after each garbage collection)
      type: bool  default: false
--trace-gc-ignore-scavenger (do not print trace line after scavenger collection)
      type: bool  default: false
--trace-idle-notification (print one trace line following each idle notification)
      type: bool  default: false
--trace-idle-notification-verbose (prints the heap state used by the idle notification)
      type: bool  default: false
--trace-gc-verbose (print more details following each garbage collection)
      type: bool  default: false
--trace-allocation-stack-interval (print stack trace after <n> free-list allocations)
      type: int  default: -1
--trace-duplicate-threshold-kb (print duplicate objects in the heap if their size is more than given threshold)
      type: int  default: 0
--trace-fragmentation (report fragmentation for old space)
      type: bool  default: false
--trace-fragmentation-verbose (report fragmentation for old space (detailed))
      type: bool  default: false
--trace-evacuation (report evacuation statistics)
      type: bool  default: false
--trace-mutator-utilization (print mutator utilization, allocation speed, gc speed)
      type: bool  default: false

--trace-parallel-scavenge (trace parallel scavenge)
      type: bool  default: false
--trace-concurrent-marking (trace concurrent marking)
      type: bool  default: false

--trace-incremental-marking (trace progress of the incremental marking)
      type: bool  default: false
--trace-stress-marking (trace stress marking progress)
      type: bool  default: false
--trace-stress-scavenge (trace stress scavenge progress)
      type: bool  default: false
--track-gc-object-stats (track object counts and memory usage)
      type: bool  default: false
--trace-gc-object-stats (trace object counts and memory usage)
      type: bool  default: false
--trace-zone-stats (trace zone memory usage)
      type: bool  default: false
--track-retaining-path (enable support for tracking retaining path)
      type: bool  default: false

--track-detached-contexts (track native contexts that are expected to be garbage collected)
      type: bool  default: true
--trace-detached-contexts (trace native contexts that are expected to be garbage collected)
      type: bool  default: false

--trace-minor-mc-parallel-marking (trace parallel marking for the young generation)
      type: bool  default: false
--minor-mc (perform young generation mark compact GCs)
      type: bool  default: false
```

### Maps

```
--trace-generalization (trace map generalization)
      type: bool  default: false
--trace-unmapper (Trace the unmapping)
      type: bool  default: false

--trace-maps (trace map creation)
      type: bool  default: false
--trace-maps-details (also log map details)
      type: bool  default: true
```

### ICs

```
--trace-ic (trace inline cache state transitions for tools/ic-processor)
      type: bool  default: false
--ic-stats (inline cache state transitions statistics)
      type: int  default: 0
```

### Optimization/Deoptimization

```
--print-deopt-stress (print number of possible deopt points)
      type: bool  default: false

--trace-opt (trace lazy optimization)
      type: bool  default: false
--trace-opt-verbose (extra verbose compilation tracing)
      type: bool  default: false
--trace-opt-stats (trace lazy optimization statistics)
      type: bool  default: false
--trace-deopt (trace optimize function deoptimization)
      type: bool  default: false
--trace-file-names (include file names in trace-opt/trace-deopt output)
      type: bool  default: false

--redirect-code-traces (output deopt information and disassembly into file code-<pid>-<isolate id>.asm)
      type: bool  default: false
--redirect-code-traces-to (output deopt information and disassembly into the given file)
      type: string  default: nullptr

--print-opt-source (print source code of optimized and inlined functions)
      type: bool  default: false
```

### Code Snapshots

```
--trace-serializer (print code serializer trace)
      type: bool  default: false
--trace-lazy-deserialization (Trace lazy deserialization.)
      type: bool  default: false

--profile-deserialization (Print the time it takes to deserialize the snapshot.)
      type: bool  default: false
--serialization-statistics (Collect statistics on serialized objects.)
      type: bool  default: false
```

### Logging

```
--log-all (Log all events to the log file.)
      type: bool  default: false
--log-api (Log API events to the log file.)
      type: bool  default: false
--log-code (Log code events to the log file without profiling.)
      type: bool  default: false
--log-handles (Log global handle events.)
      type: bool  default: false
--log-suspect (Log suspect operations.)
      type: bool  default: false
--log-source-code (Log source code.)
      type: bool  default: false
--log-function-events (Log function events (parse, compile, execute) separately.)
      type: bool  default: false
--logfile (Specify the name of the log file.)
      type: string  default: v8.log
--logfile-per-isolate (Separate log files for each isolate.)
      type: bool  default: true

--log-internal-timer-events (Time internal events.)
      type: bool  default: false
--log-timer-events (Time events including external callbacks.)
      type: bool  default: false
```

### Misc

```
--trace-interrupts (trace interrupts when they are handled)
      type: bool  default: false

--trace-compiler-dispatcher (trace compiler dispatcher activity)
      type: bool  default: false
--trace-compiler-dispatcher-jobs (trace progress of individual jobs managed by the compiler dispatcher)
      type: bool  default: false

--trace-prototype-users (Trace updates to prototype user tracking)
      type: bool  default: false
--trace-for-in-enumerate (Trace for-in enumerate slow-paths)
      type: bool  default: false
```
