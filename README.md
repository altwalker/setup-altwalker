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
      altwalker-version: '0.3.1'
  - name: Run AltWalker
    run: |
      altwalker --version

```

The `altwalker-version` input is optional. If the `altwalker-version` option does't exist the last released version of AltWalker will be installed.

See [action.yml](action.yml) for more details.

This action also provides all input options provided by [@altwalker/setup-graphwalker](https://github.com/altwalker/setup-graphwalker) action.

## License

This project is licensed under the [MIT License](LICENSE).