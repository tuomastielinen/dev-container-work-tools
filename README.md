# dev-container-work-tools

## Dev Containers

Available features can be found [here](https://containers.dev/features).

## GitHub Actions

Actions workflows need read and write permissions to push images to ghcr.io. Go to repository settings > Actions > General > Workflow permissions > select **Read and write permissions**.  

## Local Dev Container configurations

You can use local dev container configurations, so that they don't need to be pushed into shared repositories. The configurations are stored in the path: ~/.config/Code/User/globalStorage/ms-vscode-remote.remote-containers/configs/<name-of-the-directory>/.devcontainer/devcontainer.json

Here is a basic configuration file:

```json
{
	"name": "work tools - Local Configuration",
	// Or use a Dockerfile or Docker Compose file. More info: https://containers.dev/guide/dockerfile
	"image": "ghcr.io/tuomastielinen/dev-container-work-tools/devcontainer"
}
```

To open a folder in a dev container, open the command palette and select: **Dev Containers: Open Folder in Container...**. Then select the desired configuration file.