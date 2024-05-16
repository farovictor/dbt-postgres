# To install dbt-postgres in Linux

Dependency:
1. Install hatch on your machine or environment. [Installation Guide](https://hatch.pypa.io/latest/install/)
```bash
  # Installing using pip
  pip install hatch

  # check your version
  hatch --version
```

# Building Package
1. Clone this repo
```bash
  git clone https://github.com/farovictor/dbt-postgres.git
```


2. Build the thing
```bash
  # Go to project folder
  cd dbt-postgres

  # Build wheel file
  hatch build
```


3. Move the dependency to your project. Instead of installing from a repo, point the installation to the wheel file.
```bash
  # e.g.: Pip installation
  pip install dbt_postgres-1.9.0a1-py3-none-any.whl

  # e.g.: Poetry installation
  poetry add dbt_postgres-1.9.0a1-py3-none-any.whl
```

Adjust it to whatever is your package manager.

# CAVEAT

This repo is just to provide a workaround to the issue with psycopg2 installation.
Please refer to the issue link to check when the issue is resolved and keep an up-to-date version of the package.
Issue: [Issue-96](https://github.com/dbt-labs/dbt-postgres/issues/96)
