## Development Flow

### Document new feature

Write documentation about what the new feature solves and provides for the user of the package. This way we define the scope of the feature (what's included and what not), so that we can make sure that the feature is implemented in the right way. This documentation should make clear to the product manager (the client), the developer and the end user what the feature is about.

### Document api for new feature

Write down the documentation for the api. How will the feature be used by the user of the package. This is also known as documentation driven development. By writing down the api first, before implementing it, we make sure that the api is user friendly.

### Write tests and implement feature

Implement the feature by using a test driven development. Write code guided by the tests you write. Tests will be run by Github actions when pushed to origin. This will make sure future development will not break existing functionality.

### Release new version

Release a new version of the package by:

- creating a new release on Github.
- adding a tag, example: `1.1.0`.
- adding a release title, example: `v1.1.0`
- describe the changes for this release.

Packagist will automatically pick up this release.

Because we wrote documentation and tests first. Everything will be ready when we release a new version. Packagist will pick up on the new version when a new tag is used.

## Versioning

Use semantic versioning (semver)

`MAJOR`.`MINOR`.`PATCH`

- `MAJOR` version when you make incompatible API changes.
- `MINOR` version when you add functionality in a backwards compatible manner.
- `PATCH` version when you make backwards compatible bug fixes.
