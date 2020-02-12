# VSCode Extension for Topcoder

This extension is meant to closely integrate the Topcoder platform with [VSCode](https://code.visualstudio.com/), the text editor, to allow the user to perform actions related to the Topcoder platform from within the editor, without having to open a browser.

## Setup your environment

- Before you can use the extension, you need to provide your Topcoder credentials
- This extension provides two settings in this regard

```bash
TCVSCodeIDE.credentials.username: Your Topcoder username
TCVSCodeIDE.credentials.password: Your Topcoder password
```

You can also set them in your Extension specific Settings:

![Settings Credentials](/images/settings_credentials.png)

## Useful Commands

The extension provides several commands in the Command Palette:

- *Topcoder: Login* to login in Topcoder using your username and password.
- *Topcoder: Logout* to clear the stored login token.
- *Topcoder: View open challenges* to list active challenges in a tabular view. Upon clicking on a challenge title, challenge details will be displayed in a new tab.
- *Topcoder: Upload submission* to upload the current workspace to topcoder challenge.
- *Topcoder: Clone a repository* to clone a gitlab/github public repository.
- *Topcoder: Clone templates* to clone a template - available at [Topcoder Templates](https://github.com/topcoder-platform-templates)

## Activity Bar

The extensions adds an activity bar item that has 3 sections.

- *Your Active Contests*  will list all the contests that you have registered to.
- *Your Active Submissions* will list all the submissions that you have done. You will be able to view the reviews and artifacts (if any) for the submission.
- *Home* has 3 parts, which will allow you to access the extension features guide, the setup guid or the list of all active challenges respectively.

![Activity Bar](/images/activity_bar.gif)

## Features

- You can view the list of open challenges in the Topcoder platform
- You can view the details of a challenge
- You can register for open challenges
- You can initialize your workspace after registering for a challenge. This creates a `.topcoderrc` file with the challenge details present in it. This file is used by the extension and never to be altered manually
- You can also clone challenge repositories right into your workspace
- You can also clone a template repository from [Topcoder Templates](https://github.com/topcoder-platform-templates) into your workspace
- You can clone any public gitlab or github repository into your workspace
- If your workspace is initialized, you can see the time until the end of the submission phase in the side bar
- You can also see the current time (as used by the Topcoder platform, for example in Online Review) status bar
- Finally you can switch between the topcoder production and development instances

## Other Settings

Besides setting your username and password, you can also:

- Switch between the development and production instances of Topcoder when using the extension. By default, you will be using the production instance
- At the moment, we capture telemetry of your usage of this extension to help improve the extension. Although we now have a stable release, option to control telemetry did not make it to the latest release. We intend to provide this soon

These settings are named:

```bash
TCVSCodeIDE.useDevelopEndpoint: Boolean value. false by default
```

### NOTE: When any configuration is changed, you have to logout and reload your VSCode window for the changes to take effect
