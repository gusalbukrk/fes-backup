# Front-end Starter

## Known issues

### webpack-dev-server & .browserslistrc

- webpack-dev-server's auto-reloading doesn't work when there's a `.browserslistrc` file or key in package.json
- this happens because webpack-dev-server (currently in version 3.11) isn't yet 100% compatible with webpack 5, but will be in version 4
- temporarily **solution**:
  - `target: web` at `webpack.config.js`
