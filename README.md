# README.md Geni

Automatically generate `README.md` files for your JS/TS projects from their `package.json`.

## Features

- Extracts project name, version, description.
- Generates install and usage instructions.
- Easy to integrate GitHub Action.

## Usage

Add the `readme-geni` action to your GitHub Workflow:

yaml
name: Generate README
on:
  push:
    branches:
      - main
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Generate README.md
        uses: your-org/readme-geni@v1 # Replace with actual action path
        with:
          output_path: './README.md'


## Pro Version ($9.99)

Unlock custom templates and advanced configuration for a one-time purchase. See [our website](https://readme-geni.vercel.app) for details.
