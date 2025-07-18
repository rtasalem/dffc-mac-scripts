# Defra FFC Mac Scripts

Bash scripts for automating the process of setting up a MacBook for local development within Defra's FFC (Future Farming & Countryside) programme, also known as FCP (Farming & Countryside Programme). All installations are completed using [Homebrew](https://brew.sh/).  

Below is a summary of each script's purpose. It's recommended to run the scripts in the order presented in the table (excluding the `help` script):
| Script | Description | Command |
| -------------- | ------------------------------------------------------------------------------------ | ------- |
| [help](./help) | List all available commands for dffc-mac-scripts. | `./help` |
| [install](./install) | Bulk installs most of the packages required in the [ffc-development-guide](https://github.com/DEFRA/ffc-development-guide/blob/main/docs/local-development-setup/index.md) (excluding NVM (Node Version Manager) & neostandard). | `./install` |
| [version](./version) | Checks version of each package installed using the `install` script. Useful for confirming installation was successful. | `./version` |
| [optional](./optional) | Yes/no prompts to install optional packages and desktop applications that are not listed in the FFC development guide but are useful for day-to-day development: Slack, Microsoft Teams, Microsoft Outlook, Google Chrome, Obsidian, draw.io, pgAdmin 4, postgresql@14, MongoDB Compass, mongosh, Postman, Lens, K9s, Azure Data Studio, and Azure Storage Explorer, and yq. | `./optional` |
| [update](./update) | Checks and downloads any updates for Homebrew and packages installed via Homebrew. | `./update` |

All scripts can be executed from the VS Code Command Palette. To run a script, open the Command Palette (`ctrl+shift+p` or `cmd+shift+p`), select Tasks: Run Task, and choose the desired task from the list.

Important to note that some parts of the FFC development guide are _not_ covered by these scripts: Neostandard and NVM (Node Version Manager). Please refer to the [FFC Development Guide](https://github.com/DEFRA/ffc-development-guide) for full instructions.
