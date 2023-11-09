# artifact-events-infrastructure-artifact

Artifact space for <https://github.com/pythoneda-shared-artifact-changes/artifact-events-infrastructure>

## How to declare it in your flake

Check the latest tag of the artifact repository: [https://github.com/pythoneda-shared-artifact/artifact-events-infrastructure-artifact/tags](https://github.com/pythoneda-shared-artifact/artifact-events-infrastructure-artifact/tags) and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-shared-artifact-artifact-events-infrastructure-arti = {
      [optional follows]
      url =
        "github:pythoneda-shared-artifact/artifact-events-infrastructure-artifact/[version]?dir=artifact-events-infrastructure";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://github.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://github.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-shared-artifact-artifact-events-infrastructure-python38` 
- `#packages.[system].pythoneda-shared-artifact-artifact-events-infrastructure-python39` 
- `#packages.[system].pythoneda-shared-artifact-artifact-events-infrastructure-python310` 
- `#packages.[system].pythoneda-shared-artifact-artifact-events-infrastructure-python311` 

The Nix flake is under the 
[infrastructure](https://github.com/pythoneda-shared-artifact/artifact-events-infrastructure-artifact/tree/main/artifact-events-infrastructure "artifact-events-infrastructure") folder in <https://github.com/pythoneda-shared-artifact/artifact-events-infrastructure-artifact>.

