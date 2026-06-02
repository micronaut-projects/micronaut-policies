Micronaut follows [semantic versioning](https://semver.org/).

Micronaut components are versioned according to the following scheme:

```
<MAJOR>.<MINOR>.<PATCH>
```

- A new component patch version, e.g., a component going from 1.2.1 to 1.2.2, differs from the previous one only by the inclusion of bug fixes, documentation changes, or patch dependency updates.
- A new component minor version, e.g., a component going from 1.2.3 to 1.3.0, differs from the previous one by the inclusion of new features, bug fixes, documentation changes, or minor dependency updates.
- A new component major version, e.g., a component going from 1.2.3 to 2.0.0, differs from the previous one by the removal of deprecated code, the potential inclusion of breaking changes, new features, bug fixes, documentation changes, or minor dependency updates.

A patch version may include breaking changes if those changes are necessary to fix a security vulnerability. A patch version may include a transitive dependency upgrade to a minor or major version if that is necessary to fix a security vulnerability.
