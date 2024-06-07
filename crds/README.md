# How to generate the CRDs?

- Install `controller-kubernetes-tools`
- Run `controller-gen crd:ignoreUnexportedFields=true paths=./pkg/apis/pipeline/v1/ output:dir=./crds`

# How to generate the JSON schema from the crds?

- Run `nix run github:tricktron/crd2jsonschema -- -a -o jsonschemas/ crds/*.yaml`
