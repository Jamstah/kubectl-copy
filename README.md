# kubectl-copy

A kubectl plugin that copies resources from one namespace to another.

## Installation

Add the script to your path with the name `kubectl-copy`.

See the [kubectl documentation](https://kubernetes.io/docs/tasks/extend-kubectl/kubectl-plugins/#installing-kubectl-plugins) for more information.

## Usage

Run `kubectl copy` with equivalent args to `kubectl get` first, then the target namespace last.

```
jammy:~$ kubectl copy configmap -l can-select-by-label target-namespace
configmap/example1 created
configmap/example2 created
```
