---
title: Tilt CLI Reference
layout: docs
hideEditButton: true
---
## tilt alpha tiltfile-result

Exec the Tiltfile and print results as JSON (note: the API is unstable and may change)

### Synopsis

Exec the Tiltfile and print results as JSON (note: the API is unstable and may change).

Exit code 0: successful Tiltfile evaluation (JSON printed to stdout)
Exit code 1: some failure in setup, printing results, etc. (any logs printed to stderr)
Exit code 5: error when evaluating the Tiltfile, such as syntax error, illegal Tiltfile operation, etc. (any logs printed to stderr)

Run with -v | --verbose to print Tiltfile execution logs on stderr, regardless of whether there was an error.

```
tilt alpha tiltfile-result [flags]
```

### Options

```
      --file string   Path to Tiltfile (default "Tiltfile")
  -h, --help          help for tiltfile-result
```

### Options inherited from parent commands

```
  -d, --debug                          Enable debug logging
      --klog int                       Enable Kubernetes API logging. Uses klog v-levels (0-4 are debug logs, 5-9 are tracing logs)
      --log-flush-frequency duration   Maximum number of seconds between log flushes (default 5s)
      --trace                          Enable tracing
      --traceBackend string            Which tracing backend to use. Valid values are: 'windmill', 'lightstep', 'jaeger' (default "windmill")
  -v, --verbose                        Enable verbose logging
```

### SEE ALSO

* [tilt alpha](tilt_alpha.html)	 - unstable/advanced commands still in alpha

###### Auto generated by spf13/cobra on 1-Apr-2020