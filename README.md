# What is it?

Tabby is an open-source window & tab manager that can manage great amounts of windows and tabs at ease.

This is the development branch for Tabby v2.0.

You can install Tabby on it's Firefox Add-on page: https://addons.mozilla.org/en-US/firefox/addon/tabby-window-tab-manager/
Or, to install the newest development version, see the [Installing the dev build](#installing-the-dev-build) section.

# Contributing

If you like this project, please share it. Your support is always welcomed!

Tabby is an open-source project and is in active development, so feel free to submit any issues that you are experiencing and I will do my best to fix it. And if you can fix the issue altogether, feel free to submit a pull request!

My Website: http://www.WhatsYourIdea.com

# Building, Installing, and Editing

## Prerequisites

- Git
- Node.js
- Firefox >= 59 (recommended)

## Building Tabby

1. Open a git enabled shell of your choice (e.g. Command Prompt, Git Bash)
2. Get the source code  
`git clone https://github.com/Bill13579/tabby.git`
3. Go into the Tabby directory  
`cd tabby`
4. Switch to the `v2.0-dev` branch  
`git checkout v2.0-dev`
5. Install dependencies with npm  
`npm install`
6. Build Tabby  
`npm run build`

## Installation

This instruction will install Tabby as a temporary add-on, so you will need to re-do this everytime you restart Firefox.

1. Start Firefox
2. Go to `about:debugging`
3. Press on the `Load Temporary Add-on...` button
4. Select the `manifest.json` file in the `dist` directory

## Editing & Testing

After you edit the code, you will need to build again.

Re-do step 6 of [Building Tabby](#building-tabby) and press the `Reload` button in the Tabby section of the `about:debugging` page.

Note: Content Scripts will only be reloaded for each tab once that tab is refreshed.

# File Structure

icons/ - Directory for storing Tabby icons<br/>
icons/tabby.svg - Tabby icon (Vector)<br/>
icons/tabby.png - Tabby icon (Raster)<br/>

release/ - Release zip files<br/>

screenshots/ - Screenshots<br/>
screenshots-archive/ - Old screenshots of old releases<br/>

src/ - Source code directory<br/>

src/ - Firefox source code directory<br/>
src/content/ - Tabby content scripts<br/>
src/icons/ - Icons used in the Tabby UI<br/>
src/popup/ - Tabby popup scripts<br/>
src/popup/index.html - Tabby popup main html file<br/>
src/popup/popup.css - Tabby popup main css file<br/>
src/popup/popup.js - Tabby popup main javascript file<br/>
src/background.js - Tabby background script<br/>
src/manifest.json - Web extension manifest file<br/>

LICENSE - License file<br/>
README.md - README file
