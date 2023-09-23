# setup-altwalker

Set up your GitHub Actions workflow with a specific version of AltWalker.

This action provides the following functionality for GitHub Actions users:

* Installing a version of Python or PyPy
* Installing a version of Java
* Installing a version of GraphWalker CLI and (by default) adding it to the `PATH`
* Installing a version of AltWalker

## Usage

```yml
steps:
  - name: Setup AltWalker
    uses: altwalker/setup-altwalker@v1
    with:
      altwalker-version: '0.4.0'
  - name: Run AltWalker
    run: |
      altwalker --version

```

The `altwalker-version` input is optional. If the `altwalker-version` option is not specified, the latest released version of AltWalker will be installed.

For additional details, refer to [action.yml](action.yml).

Furthermore, this action offers all the input options available in the [altwalker/setup-graphwalker](https://github.com/altwalker/setup-graphwalker) action.

## License

This project is licensed under the [MIT License](LICENSE).
