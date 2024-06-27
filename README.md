<div align="center">
  <img src="https://ai4eosc.eu/wp-content/uploads/sites/10/2022/09/horizontal-transparent.png" alt="logo" width="500"/>
</div>

# AI4OS Tools catalog

[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)

This catalog gathers all the AI tools integrated in the AI4OS Marketplace.
AI tools are listed as git submodules.


### Adding a tool to the catalog

To add a tool to the catalog:
```bash
git submodule add https://github.com/ai4os/<tool_name>
```

If the user has a default branch different from `master` (eg. `main`),
you should add this parameter in the submodule command:

```bash
git submodule add -b main https://github.com/ai4os/<tool_name>
```

### Removing a tool from the catalog

To remove a tool from the catalog:
```bash
bash utils/remove-submodule.sh <tool_name>
```

### Updating the existing tools

To update the existing tools:
```bash
git pull --recurse-submodules
git submodule update --remote --recursive
```
