<!-- SPDX-FileCopyrightText: © 2026 Jeffrey C. Ollie <jeff@ocjtech.us> -->
<!-- SPDX-License-Identifier: MIT -->


# Install the Nix package manager on your Buildkite agent

## Example

```yml
steps:
  - command: nix run nixpkgs#hello
    plugins:
      - jcollie/install-nix#v1.1.0
```

### Configuration

### Developing

To run the tests:

```shell
podman run -it --rm -v "$PWD:/plugin:ro" docker.io/buildkite/plugin-linter --id jcollie/install-nix
```
