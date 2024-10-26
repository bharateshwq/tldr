# npm deprecate

> Deprecate a version of a package.
> More information: <https://docs.npmjs.com/cli/npm-deprecate>.

- Deprecate a package version - Updates the npm registry entry for a package, providing a deprecation warning to all who attempt to install it like this `npm deprecate my-thing@"< 0.2.3" "critical bug fixed in v0.2.3"`:

`npm deprecate <package-spec> <message>`

- Deprecate a version range - Works on version ranges as well as specific versions. This will also deprecate prerelease versions like `my-thing@1.0.0-beta.0`.:

`npm deprecate my-thing@1.x "1.x is no longer supported"`

- Undeprecate a package - To remove a deprecation, specify an empty string for the message argument:

`npm deprecate <package-spec> ""`
