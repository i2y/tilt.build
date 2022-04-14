---
title: Tilt CLI Reference
layout: docs
sidebar: reference
hideEditButton: true
---
## tilt lsp start

Start the Starlark LSP server

### Synopsis

Start the Starlark LSP server.

By default, the server will run in stdio mode: requests should be written to
stdin and responses will be written to stdout. (All logging is _always_ done
to stderr.)

For socket mode, pass the --address option.


```
tilt lsp start [flags]
```

### Examples

```

# Launch in stdio mode with extra logging
tilt lsp start --verbose

# Listen on all interfaces on port 8765
tilt lsp start --address=":8765"

```

### Options

```
      --address string   Address (hostname:port) to listen on
  -h, --help             help for start
```

### Options inherited from parent commands

```
      --debug      Enable debug logging
      --klog int   Enable Kubernetes API logging. Uses klog v-levels (0-4 are debug logs, 5-9 are tracing logs)
      --verbose    Enable verbose logging
```

### SEE ALSO

* [tilt lsp](tilt_lsp.html)	 - Language server for Starlark

###### Auto generated by spf13/cobra on 8-Apr-2022