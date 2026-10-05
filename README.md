# transport-minizinc-mcp

A Model Context Protocol server that validates and solves constraint models written in the MiniZinc modelling language.

## What it is for

It gives an agent two tools, one that type-checks a model and one that solves it. Each takes the model and optional data as text and returns the result as JSON. The server calls the `minizinc` command-line tool to do the work.

## Build and run

The `minizinc` tool must be on the path; the container image installs it.

```sh
mix deps.get
mix mcp.server
```

`docker build .` builds the container image.

## Licence

MIT; see LICENSE.md.
