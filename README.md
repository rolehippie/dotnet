# dotnet

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/dotnet) [![Testing Build](https://github.com/rolehippie/dotnet/workflows/testing/badge.svg)](https://github.com/rolehippie/dotnet/actions?query=workflow%3Atesting) [![Readme Build](https://github.com/rolehippie/dotnet/workflows/readme/badge.svg)](https://github.com/rolehippie/dotnet/actions?query=workflow%3Areadme) [![Galaxy Build](https://github.com/rolehippie/dotnet/workflows/galaxy/badge.svg)](https://github.com/rolehippie/dotnet/actions?query=workflow%3Agalaxy) [![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/dotnet)](https://github.com/rolehippie/dotnet/blob/master/LICENSE) 

Ansible role to install .NET packages from Microsoft repos. 

## Sponsor 

[![Proact Deutschland GmbH](https://proact.eu/wp-content/uploads/2020/03/proact-logo.png)](https://proact.eu) 

Building and improving this Ansible role have been sponsored by my employer **Proact Deutschland GmbH**.

## Table of content

* [Default Variables](#default-variables)
  * [dotnet_packages](#dotnet_packages)
  * [dotnet_repo_distribution](#dotnet_repo_distribution)
  * [dotnet_repo_release](#dotnet_repo_release)
  * [dotnet_repo_version](#dotnet_repo_version)
* [Dependencies](#dependencies)
* [License](#license)
* [Author](#author)

---

## Default Variables

### dotnet_packages

List of packages to install

#### Default value

```YAML
dotnet_packages:
  - dotnet-runtime-3.1
  - aspnetcore-runtime-3.1
```

### dotnet_repo_distribution

Enforce another distribution for the repo

#### Default value

```YAML
dotnet_repo_distribution: '{{ ansible_distribution | lower }}'
```

### dotnet_repo_release

Enforce another release for the repo

#### Default value

```YAML
dotnet_repo_release: '{{ ansible_distribution_release }}'
```

### dotnet_repo_version

Enforce another version for the repo

#### Default value

```YAML
dotnet_repo_version: '{{ ansible_distribution_version }}'
```

## Dependencies

* [rolehippie.docker](https://github.com/rolehippie/docker)

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
