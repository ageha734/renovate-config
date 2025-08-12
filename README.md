Here is the English version of the README.md, revised for an open-source project.

## Shared Renovate Configuration

This repository provides a shared Renovate configuration for use across multiple products. The goal is to minimize technical debt by continuously tracking library updates and maintaining the latest dependencies.

### How to Inherit and Use

To use this shared configuration, follow these steps in your repository:

1.  **Enable Renovate**
    Enable Renovate for your repository.

2.  **Create a Configuration File**
    Create a `renovate.json` file in the root directory of your project and extend the shared configuration like this:

    ```json
    {
      "extends": [
        "github>ageha734/renovate-config"
      ],
      "enabledManagers": ["npm"]
    }
    ```

    Be sure to set `"enabledManagers"` to match the package manager(s) used in your project.

-----

### Customizing the Configuration

If you need to override the shared settings or add your own rules, simply add the desired configuration options to your `renovate.json` file.

For a full list of available options, please refer to the official Renovate documentation:
[Configuration Options - Renovate Docs](https://docs.renovatebot.com/configuration-options/)

We hope this configuration helps keep your projects running smoothly. If you have any questions or suggestions for improvement, feel free to create an issue or a pull request.
