# Defra FFC Mac Scripts

Scripts for automating the process of setting up a MacBook for local development within Defra's FFC (Future Farming & Countryside) programme, also known as FCP (Farming & Countryside Programme). All installations are completed via [Homebrew](https://brew.sh/)<br>

Below is a summary of each script's purpose (it's recommended to run the scripts in the order presented in the table):
| Script | Description | Command |
| -------------- | ------------------------------------------------------------------------------------ | ------- |
| [mandatory](./mandatory) | Bulk installs most of the packages required in the [ffc-development-guide](https://github.com/DEFRA/ffc-development-guide/blob/main/docs/local-development-setup/index.md). Installs Command Line Tools for Xcode, Homebrew, kubectl, Azure CLI, Helm, Snyk CLI, GitHub CLI, Python, Pip, pre-commit, detect-secrets, .NET SDK, Docker, Visual Studio Code.  | `./mandatory` |
| [version](./version) | Checks version of each package installed using the `mandatory` script. | `./version` |
| [optional](./optional) | Yes/no prompts to install optional packages and desktop applications that are not listed in the FFC development guide but are useful for day-to-day development: Slack, Microsoft Teams, Microsoft Outlook, Google Chrome, Obsidian, draw.io, pgAdmin 4, postgresql@14, MongoDB Compass, mongosh, Postman, Lens, K9s, Azure Data Studio, and Azure Storage Explorer, and yq | `./optional` |

Important to note that some parts of the FFC development guide are _not_ covered by these scripts: StandardJS and NVM (Node Version Manager). Please refer to the [FFC Development Guide](https://github.com/DEFRA/ffc-development-guide) for full instructions.
