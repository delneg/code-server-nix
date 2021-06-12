## Code-server service for NixOS


### Usage:

```
imports =
    [
      # Include the results of the hardware scan.
      ./hardware-configuration.nix
      # Import this file
      ./code-server.nix
    ];
```

```
service.code-server = {
        enable = true;
        host = "0.0.0.0";
        user = "username";
    };
```

The default port is 5092.

Credit goes to https://github.com/christoph00

