# How to generate the CRDs?

- Install `controller-kubernetes-tools`
- Run `controller-gen crd:ignoreUnexportedFields=true paths=./pkg/apis/pipeline/v1/ output:dir=./crds`
