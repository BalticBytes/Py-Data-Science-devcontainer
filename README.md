# Python Data Science devcontainer

A minimal working setup providing a devcontainer for vscode + python + jupyter notebooks.

## Sources / Prerequisites

- [vscode](https://code.visualstudio.com/)
- [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension for vscode
- [Docker + docker-compose](https://www.docker.com/get-started)
  - Image: [amalic/jupyterlab](https://hub.docker.com/r/amalic/jupyterlab)
  - Found in [this repository](https://github.com/amalic/Jupyterlab) by [@amalic](https://github.com/amalic)

## Usage

1. Install vscode and the Remote - Containers extension
2. Click on the small green button >< on the bottom left of vscode **OR** (ctrl+p)
3. Type and choose `>Remote-Containers: Reopen in Container`

## Notes
Changing the current working directory (cwd) enables you to utilize relative imports in your jupyter notebook.

Example (included in repo): 
- Local Module (src/util.py)
- Notebook (src/example.ipynb)
```python
# This needs to be ran to make relative imports work
import os
os.chdir("/workspaces")
os.getcwd()
```

## License

MIT