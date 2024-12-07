# Jupyter Notebooks

My personal JupyterLite setup that's deployed as a static site. You can find out more about this [here](https://jupyterlite.readthedocs.io/en/stable/quickstart/deploy.html).

This has been deployed [here](https://ng-jupyter.dev).

## Install micromamba

```bash
brew install micromamba
```

## Confirm everything is installed

```bash
jupyter lite --version
```

This should output something like `0.4.5`.

## Build the site

```bash
jupyter lite build --contents content --output-dir dist
```

## Serve the site

```bash
npx serve dist
```

It should then be available on `http://localhost:3000`.

## Exporting new requirements

```bash
uv export --format requirements-txt > ./requirements.txt
```