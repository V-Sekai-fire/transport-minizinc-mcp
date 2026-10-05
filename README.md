# transport-minizinc-mcp

A Model Context Protocol server that validates and solves constraint models written in the MiniZinc modelling language.

## What it is for

It gives an agent tools that type-check a model, solve it, and list the installed solvers. The model and optional data go in as text and the result comes back as JSON. The server calls the `minizinc` command-line tool to do the work.

## Build and run

The `minizinc` tool must be on the path; the container image installs it.

```sh
mix deps.get
mix mcp.server
```

`docker build .` builds the container image.

## Licence

MIT; see LICENSE.md.
