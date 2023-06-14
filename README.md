# Empty package

This empty package is designed to be used as a placeholder in package managers.

It contains no code or functionality, and exists simply to serve as a reference in dependency management.

Including this package in your project can be advantageous if you aim to restrict the installation of specific packages or need to verify your package manager's configuration.

## Usage

To use this package as a placeholder, you can reference it in your package manager configuration files.

For instance, if you're using pnpm, you can override a particular package by including the following in your package.json file:

```json
{
  "pnpm": {
    "overrides": {
      "pg-native": "npm:voidage",
      "libpq": "npm:voidage"
    }
  }
}
```

By doing so, pnpm will resolve `pg-native` and `libpq` to `voidage`, rather than installing the actual packages.

This can be useful if you want to prevent certain packages from being installed, or if you need to test your package manager's configuration.

## Disclaimer

The code for this package can be reviewed at [https://unpkg.com/voidage/](https://unpkg.com/voidage/), which demonstrates that it does not contain any known security vulnerabilities or malicious code.
