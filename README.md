[![build and tests](https://github.com/lukka/set-shell-env/workflows/build-test/badge.svg)](https://github.com/lukka/set-shell-env)

# [**set-shell-env** action ](https://github.com/marketplace/actions/run-cmake)

This action exports as GitHub's variables all the shell environment variables. After its execution any environment variable is accessible by using `${{ env.<VARIABLENAME> }}`.

 ## User Manual
 * [Quickstart](#quickstart)
 * [Action reference: all input/output parameters](#reference)
 
 ## Developer Manual
 * [Developers information](#developers-information)
   * [Prerequisites](#prerequisites)
   * [Packaging](#packaging)
   * [Testing](#testing)
  * [Contributing](#contributing)
  * [License](#license)

## <a id='quickstart'>Quickstart</a>

```yaml
    - uses: lukka/set-shell-env@v0
    # with:
    #   shell: 'bash' or 'tcsh' or any command that starts a shell .
    #   args: '-c env' or any arguments that print out the environment variables as pairs of: NAME=VALUE .
    #   filter: '.*' is the default, i.e. include all by default.
    #   includeFilter: indicates if the filter includes or exclude variables.
    #  Here onward any following step can access any environment variable using:
    #  in your yml file:
    #     ${{ env.NAME }}
```

### <a id='reference'>Action reference: all input/output parameters</a>

[action.yml](https://github.com/lukka/set-shell-env/blob/v0/action.yml)

# Developers information

## Prerequisites
[gulp 4](https://www.npmjs.com/package/gulp4) globally installed.

## Build and lint
Build with `tsc` running:

 > npm run build

Launch `lint` by:

 > npm run lint

## Packaging
To build, lint validate and package the extension for release purpose, run:

  > npm run pack

## Testing

To build, pack and test:
 
 > npm run test

 To run test directly:
 
 > jest

## <a id='contributing'>Contributing</a>

The software is provided as is, there is no warranty of any kind. All users are encouraged to improve the [source code](https://github.com/lukka/set-shell-env) with fixes and new features.

# License
All the content in this repository is licensed under the [MIT License](LICENSE.txt).

Copyright (c) 2020 Luca Cappa