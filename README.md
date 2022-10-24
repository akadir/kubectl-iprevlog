<h1 align="center"><img src="icon.png"> kubectl-iprevlog</h1>

<div align="center">
Script to interactively select Deployment|ReplicaSet to print logs produced by previous containers under the selected resource.
</div>

<br>

# Installation

- Install `kubectl`, `stern`, `jq`, `fzf`.
- Download [`kubectl-iprevlog`](./kubectl-iprevlog) and save somewhere under the `$PATH` as executable file.

# Usage

```sh
kubectl-iprevlog

Print previous container logs of selected resource.

Usage:
 kubectl-iprevlog
 kubectl-iprevlog -h
 kubectl-iprevlog -r
 kubectl-iprevlog -l 15
 kubectl-iprevlog -r -l 15

Flags:
  -l number of lines    Default: 20
  -r kind               Use replicasets to select resource. Default: deployment
  -h help               Prints this help

Dependencies:

 - kubectl: https://kubernetes.io/docs/tasks/tools/install-kubectl/
 - jq: https://stedolan.github.io/jq/download/
 - fzf: https://github.com/junegunn/fzf
 - awk
```